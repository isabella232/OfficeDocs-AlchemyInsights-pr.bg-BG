---
title: Устройство в чакащо състояние
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330361"
---
# <a name="device-in-pending-state"></a>Устройство в чакащо състояние

**Предварителни изисквания:**

1. Ако настройвате регистрации на устройства за първи път, уверете се, че сте прегледали Въведение в управлението на [устройства в Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) което ще ви насочи как да получите устройства под контрола на Azure AD.
2. Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, ще трябва да [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) се уверите, че първо сте конфигурирали [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и че лицензирането е на първо място.
3. Уверете се, че сте упълномощени да извършвате операции в Azure AD и локалната AD. Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства. Освен това, ако настройвате автоматични регистрации във вашия локален Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).

Процесът на регистриране на съединението на Azure AD изисква устройствата да са в корпоративна мрежа. Тя работи и през VPN, но има някои изказ за това. Чухме, че клиентите се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридно присъединяване към Azure AD при отдалечени работни обстоятелства.

**Среда за удостоверяване в облака (с помощта на синхронизиране на хашта на пароли на Azure AD или удостоверяване чрез преминаване)**

Този регистрационен поток е известен също като "Присъединяване за синхронизиране".

Ето разбивка на това, което се случва по време на процеса на регистрация:

1. Windows 10 открива запис на точка на свързване на услугата (SCP), когато потребителят влиза в устройството.

    1. Устройството първо се опитва да извлече информация за клиента от SCP на клиента в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. За повече информация вж. [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ако е неуспешно, устройството комуникира с локалния Active Directory, за да получи информация за клиента от SCP. За да проверите SCP, вижте [този документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    **Забележка:** Препоръчваме да разрешите SCP в Active Directory и да използвате само SCP на клиента за първоначална проверка.

2. Windows 10 се опитва да комуникира с Azure AD под контекста на системата, за да се удостовери срещу Azure AD.

    Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на скрипта [за свързване чрез проверка на регистрирането на устройства](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локалния Active Directory. Това изисква ред на зрението към домейновия контролер.

4. Обектът на устройството, който има сертификат, се синхронизира с Azure AD чрез Azure AD Свързване. Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но зависи от конфигурацията на Azure AD Свързване. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. На този етап би трябвало да можете да видите устройството за тема в състояние **"Чакащо"** под "Острие на устройството" на портала на Azure.

6. При следващото потребителско влизане в Windows 10 регистрацията ще бъде завършена.

    **Забележка:** Ако сте във VPN и излизането/влизането прекратява връзката с домейна, можете да задействате регистрацията ръчно. За да направите това:
    
    Издавайте `dsregcmd /join` локално подкана за администратор или отдалечено чрез PSExec на вашия компютър.\
    Например: `PsExec -s \\win10client01 cmd, dsregcmd /join`

За често срещани проблеми с Azure Active Directory на устройства вижте [ЧЗВ за устройства.](https://docs.microsoft.com/azure/active-directory/devices/faq)
