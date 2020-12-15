---
title: Устройството в очакване на състоянието
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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/11/2020
ms.locfileid: "49676931"
---
# <a name="device-in-pending-state"></a>Устройството в очакване на състоянието

**Предпоставки**

1. Ако настройвате регистрации на устройства за първи път, моля, уверете се, че сте прегледали [въвеждането на управление на устройства в Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , което ще ви упъти как да получите устройства под контрола на Azure ad.
2. Ако регистрирате устройства в Azure AD директно и ги запишете в [неконфигурирани](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) настройки, трябва да се уверите, че сте конфигурирали предварително и имате първо [лицензите](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Уверете се, че имате разрешение за извършване на операции в Azure AD и локална реклама. Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства. Освен това, ако настройвате автоматични регистрации във вашия локален указател Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).

Процесът на регистрация за съединение на Azure AD изисква устройства за включване в корпоративна мрежа. Той работи и по VPN, но има някои ограничения за това. Чухме клиенти, които се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридната Azure AD при отдалечени работни обстоятелства.

**Среда за удостоверяване в облака (чрез хеширане при синхронизиране на Azure AD или предавано удостоверяване)**

Този регистрационен поток е известен също като "съединение за синхронизиране".

Ето разбивка на това, което се случва по време на процеса на регистриране:

1. Windows 10 включва запис за точка на свързване на услугата (SCP), когато потребителят влезе в устройството.

    1. Устройството първо се опитва да извлече информация за клиента от SCP за клиенти в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. За повече информация вижте [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ако то е неуспешно, устройството комуникира с локалния указател Active Directory, за да получи информация за клиента от SCP. За да потвърдите SCP, прегледайте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Препоръчваме ви да разрешавате SCP в Active Directory и да използвате само от страна на клиента SCP за първоначална проверка.

2. Windows 10 се опитва да комуникира с Azure AD под системен контекст за удостоверяване срещу Azure AD.

    Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на [скрипта за свързване на регистрационни устройства за проверка на устройството](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локален Active Directory. Това изисква наблюдение на домейни за администратора.

4. Обект на устройство, който има сертификат, се синхронизира с Azure AD чрез Azure AD Connect. Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но това зависи от конфигурацията на Azure AD Connect. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. На този етап би трябвало да можете да виждате устройството за теми в състояние "**Чакащо**" под "Блейд" на портала на Azure.

6. При следващото влизане в Windows 10 регистрацията ще бъде завършена.

    > [!NOTE]
    > Ако сте на VPN и излизане/влизане прекратява връзката за домейна, можете да активирате регистрацията ръчно. За да направите това:
    >
    > Издайте `dsregcmd /join` запитване локално в Админ или отдалечено чрез PSExec на вашия компютър.
    >
    > Например: `PsExec -s \\win10client01 cmd, dsregcmd /join`

За често срещани проблеми с регистрацията на устройства с Azure Active Directory вижте [ЧЗВ](https://docs.microsoft.com/azure/active-directory/devices/faq)за устройството.
