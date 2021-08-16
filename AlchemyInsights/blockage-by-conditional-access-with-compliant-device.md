---
title: Блокиран съм от условен достъп със съвместимо устройство
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
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019137"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Блокиран съм от условен достъп със съвместимо устройство

**Силно препоръчителни инструменти**

- [Инструмент за отстраняване на неизправности при регистриране на](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) устройства – изчерпателен инструмент, който помага за отстраняването на най-често срещаните проблеми с регистрирането на устройства.
- [Скрипт за свързване на регистриране на устройства](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – инструмент, който се използва, за да се гарантира, че едно устройство има достъп до крайни точки за регистриране на устройства под системния акаунт.
- [Скрипт за почистване на устройства на Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – инструмент, използван за търсене и управление на застояли устройства във вашата среда.

Ето някои често срещани причини, поради които условен достъп може да е неуспешен за съвместимо устройство или защо потребителите ви може да получават Не можете да стигнете до там от **тук** съобщение по време на заявка за влизане в организационно ресурс.

1. **Устройството не е в задължително състояние на устройството с MDM:**

Проверете дали устройството е записано при одобрен доставчик на MDM, като например Intune, *и е маркирано като съвместимо.* За повече информация за Intune вж. този [документ](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). За по-добро разбиране на съответствието на устройствата и Intune вижте Използване на правила за съответствие за задаване на [правила за устройствата, които управлявате с Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Ако имате проблеми със записването на устройство с Intune, намерете подробни данни за отстраняване на неизправности в Отстраняване на неизправности [при записване на устройство в Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). За допълнителна поддръжка на Intune създайте заявка за поддръжка. За да направите това, посетете [страницата Помощ и поддръжка на Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Устройството не е присъединено към мрежата на организацията:**

За достъп до организационни ресурси устройството трябва да бъде свързано към мрежата на организацията чрез директна връзка или виртуална частна мрежа (VPN), а също и да е присъединено към локална или Azure Active Directory. За да се присъедините към работно устройство към мрежата на организацията, вижте Присъединяване към вашето работно [устройство към мрежата на вашата организация.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) За да регистрирате лично/BYOD устройство, вижте [Регистриране на вашето лично устройство в мрежата на вашата организация.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- За да проверите дали устройството се е присъединило към мрежата, можете да следвате стъпките за регистрирани устройства [тук,](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) или да работите с [устройства тук.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) За да обхвата на проблема с мрежовата връзка на Org, следвайте указанията по-долу:

    1. Влезте, за Windows използвате своя работен или учебен акаунт, например alain@contoso.com.
    2. Свързване мрежата на вашата организация чрез VPN или DirectAccess.
    3. След като сте свързани, натиснете клавиша **с емблемата Windows+L, за** да заключите устройството.
    4. Отключете устройството си с помощта на вашия работен или учебен акаунт и след това опитайте отново да получите достъп до проблемното приложение или услуга.

Ако видите отново **съобщението за грешка Не** можете да стигнете дотук, проблемът вероятно е някъде другаде.

3. **Операционната система не се поддържа:**

Уверете се, че изпълнявате поддържана версия на операционната система, включително:

- **Windows клиент**: Windows 7 или по-нова версия

- **Windows сървър**: Windows Server 2008 R2 или по-нова версия

- **macOS**: macOS X или по-нова версия

- **Android и iOS**: Най-новата версия на мобилните операционни системи Android и iOS

4. **Уеб браузърът не се поддържа:**

Намерете поддържаните браузъри по-долу. За поддръжка на Chrome с Windows 1703 или по-нови версии се изисква Windows 10 за акаунти. За Edge 85+потребителят трябва да е влезли, за да предаде правилно информацията за съответствие на устройството. За повече подробности вижте [тук](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **iOS**: Microsoft Edge, управляван браузър Intune, Safari
- **Android**: **Microsoft Edge**: Браузър, управляван от Intune, Chrome
- **Windows Phone**: Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS:** Chrome, Safari

Намерете повече информация за стъпките за **съобщение и** отстраняване на неизправности в съобщението не можете да получите [тук.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
