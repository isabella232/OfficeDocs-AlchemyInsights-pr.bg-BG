---
title: Отстраняване на проблеми с PRT проблема
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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573323"
---
# <a name="troubleshoot-prt-issue"></a>Отстраняване на проблеми с PRT проблема

За да завърши удостоверяването на всяко устройство, то трябва да бъде напълно регистрирано и да е в добро състояние и да може да получи първоначален маркер за обновяване (PRT).

Процесът на регистрация в Azure AD съединение изисква устройства за включване в корпоративна мрежа. Той работи и по VPN, но има някои ограничения за това. Чухме за потребителите, които се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридната Azure AD при отдалечени работни обстоятелства. Ето разбивка на това, което се случва под капака, по време на процеса на регистрация.

**Среда за удостоверяване в облака (чрез хеширане при синхронизиране на Azure AD или предавано удостоверяване)**

Този регистрационен поток е известен също като "съединение за синхронизиране".

1. Windows 10 открие SCP запис при влизане на потребителя в устройството.
    1. Устройството първо се опитва да извлече информация за клиента от SCP за клиенти в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ако то е неуспешно, устройството комуникира с локалния указател Active Directory (AD), за да получи информация за клиента от точка на свързване на услугата (SCP). За да потвърдите SCP, вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Препоръчваме ви да разрешавате SCP в ОБЯВата и да използвате само от страна на клиента SCP за първоначална проверка.

2. Windows 10 се опитва да комуникира с Azure AD под системен контекст за удостоверяване срещу Azure AD. Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на скрипта за свързване на регистрационни устройства за проверка на устройството.

3. Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локалната реклама. Това изисква наблюдение на домейни за администратора.

4. Обект на устройство, който има сертификат, се синхронизира с Azure AD чрез Azure AD Connect. Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но това зависи от конфигурацията на Azure AD Connect. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. На този етап би трябвало да можете да виждате устройството за теми в състояние "Чакащо" под "Блейд" на портала на Azure.

6. При следващото влизане в Windows 10 регистрацията ще бъде завършена. 

> [!NOTE]
> Ако сте в VPN и процесът на излизане при влизане приключи със свързването на домейна, можете да активирате регистрацията ръчно:
 1. Издайте на dsregcmd/JOIN локално в Админ подкана или отдалечено чрез PSExec на вашия компютър. Например PsExec-s \\ win10client01 CMD, dsregcmd/JOIN

 2. За повече информация относно хибридните проблеми при съединението вижте [отстраняване на](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)проблеми с устройства.
