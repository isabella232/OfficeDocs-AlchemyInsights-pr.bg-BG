---
title: Блокиран съм чрез условен достъп с съвместимо устройство
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034901"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Блокиран съм чрез условен достъп с съвместимо устройство

**Силно Препоръчителни инструменти**

- [Инструмент за отстраняване на неизправности при регистриране на устройства](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – изчерпателен инструмент, който помага за отстраняване на най-често срещаните проблеми с регистрацията на устройства.
- [Скрипт за свързване на регистрационни устройства](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – инструмент, който се използва, за да се гарантира, че устройството има достъп до крайните точки за регистрация на устройства под системния акаунт.
- [Скрипт за изчистване на AZURE ad Device](https://github.com/mzmaili/AzureADDeviceCleanup) – инструмент, използван за търсене и управление на изхабени устройства във вашата среда.

Ето някои често срещани причини, поради които условният достъп може да е неуспешно за съвместимо устройство или защо вашите потребители могат да получават съобщение **, че не можете да получите достъп до него** по време на заявка за влизане в организационен ресурс.

1. **Устройството не е в задължително състояние на устройство с MDM**:

Проверете дали устройството е записано с одобрен доставчик на MDM, като например " *подчертане" и обозначен като съвместим*. За повече информация за това как да се настрои вижте този [документ](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). За по-добра яснота относно съответствието и настройката на устройството вижте [използване на правила за съответствие, за да задавате правила за устройствата, с които работите](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Ако имате проблеми при записването на устройство с добавка, вижте подробности за отстраняване на неизправности при [записване на устройство в Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). За по-нататъшна поддръжка на настройките Създайте искане за поддръжка. За да направите това, посетете [страницата за помощ и поддръжка](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)на екрана.

2. **Устройството не е присъединен към мрежата на организациите**.

За достъп до организационни ресурси устройството трябва да бъде свързано към мрежата на организацията чрез директна връзка или чрез виртуална лична мрежа (VPN), а също и към локална или Azure Active Directory. За да се присъедините към работно устройство към организационната мрежа, вижте присъединяване към устройството [за работа към мрежата на вашата организация](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). За да регистрирате лично/BYOD устройство, вижте [регистрирайте личното си устройство в мрежата на вашата организация](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- За да проверите дали устройството е присъединен към мрежата, можете да следвате стъпките за регистрирани устройства [тук](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) или служебни устройства [.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) За да обобщите проблема с мрежовата връзка на org, следвайте указанията по-долу:

    1. Влезте в Windows със своя служебен или учебен акаунт, например alain@contoso.com.
    2. Свържете се с мрежата на вашата организация чрез VPN или DirectAccess.
    3. След като сте свързани, натиснете **клавиша с емблемата на Windows + L** , за да заключите устройството си.
    4. Отключете устройството си с помощта на своя служебен или учебен акаунт и след това се опитайте да влезете отново в проблемното приложение или услуга.

Ако видите съобщение за грешка, **че не можете да стигнете до там оттук** , проблемът е вероятно другаде.

3. **Операционна система не се поддържа**:

Уверете се, че изпълнявате поддържана версия на операционната система, включително:

- **Клиент на Windows**: Windows 7 или по-нова версия

- **Windows Server**: windows Server 2008 R2 или по-нова версия

- **MacOS**: MacOS X или по-нова версия

- **Android и IOS**: най-новата версия на операционната система Android и IOS Mobile

4. **Уеб браузърът не се поддържа**:

Вижте поддържани браузъри по-долу. За поддръжка на Chrome с Windows 1703 или по-нови версии е необходимо разширение на акаунти за Windows 10. За Edge 85 + потребителят трябва да бъде влязъл в правилната информация за съответствие на устройството. За повече информация вижте [тук](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **IOS**: Microsoft Edge, браузър за управлявано управление, Safari
- **Android**: **Microsoft Edge**: Настройване на управляван браузър, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **MacOS**: Chrome, Safari

Вижте повече информация за тези стъпки **не можете да получите** съобщение и отстраняване на неизправности [тук](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
