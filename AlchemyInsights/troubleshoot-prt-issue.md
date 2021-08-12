---
title: Отстраняване на проблеми с PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972705"
---
# <a name="troubleshoot-prt-issue"></a>Отстраняване на проблеми с PRT

За да може всяко устройство да завърши удостоверяването, то трябва да бъде напълно регистрирано и в добро състояние и да може да придобие маркер за основно обновяване (PRT).

Процесът на регистриране на съединението на Azure AD изисква устройствата да са в корпоративна мрежа. Тя работи и през VPN, но има някои изказ за това. Чухме, че клиентите се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридно присъединяване към Azure AD при обстоятелства, свързани с отдалечена работа. Ето разбивка на това, което се случва "под капака" по време на процеса на регистрация.

**Среда за удостоверяване в облака (с помощта на синхронизиране на хашта на пароли на Azure AD или удостоверяване чрез преминаване)**

Този регистрационен поток е известен също като "Присъединяване за синхронизиране".

1. Windows 10 открива SCP запис при влизане на потребителя в устройството.
    1. Устройството първо се опитва да извлече информация за клиента от SCP на клиента в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ако е неуспешно, устройството комуникира с локалния Active Directory (AD), за да получи информация за клиента от точката на свързване на услугата (SCP). За да проверите SCP, вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Препоръчваме да разрешите SCP в AD и да използвате само SCP от страната на клиента за първоначална проверка.

2. Windows 10 се опитва да комуникира с Azure AD под контекста на системата, за да се удостовери срещу Azure AD. Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на скрипта за свързване чрез проверка на регистрирането на устройства.

3. Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локалната РЕКЛАМА. Това изисква ред на зрението към домейновия контролер.

4. Обект на устройство, който има сертификат, се синхронизира с Azure AD чрез Azure AD Свързване. Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но зависи от конфигурацията на Azure AD Свързване. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. На този етап би трябвало да можете да видите устройството за тема в състояние "Чакащо" под "Острие на устройството" на портала на Azure.

6. При следващото потребителско влизане в Windows 10 регистрацията ще бъде завършена. 

> [!NOTE]
> Ако сте в VPN и процесът на влизане при излизане прекратява свързването на домейна, можете да задействате регистрацията ръчно:
 1. Издавайте dsregcmd /join locally on admin prompt or remotely чрез PSExec на вашия компютър. Например PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. За повече подробности относно проблемите с хибридното присъединяване вижте Отстраняване [на проблеми с устройства](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
