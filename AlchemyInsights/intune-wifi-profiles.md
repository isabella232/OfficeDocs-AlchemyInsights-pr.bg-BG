---
title: Intune Wi-Fi профили
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554788"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi профили

Успешното внедряване на Wi-Fi свързаност за MDM клиенти зависи от правилно разположен профил, който отразява изискванията на корпоративната Wi-Fi инфраструктура. За да прегледате подходящите настройки за клиентските платформи, които проучвате, вижте: 

[Добавяне на wi-Fi настройки за устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Добавете Wi-Fi настройки за android Enterprise специализирани и напълно управлявани устройства в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Добавяне на Wi-Fi настройки за iOS и iPadOS устройства в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Добавяне на Wi-Fi настройки за Windows 10 и по-нови устройства в Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Импортиране на Wi-Fi настройки за устройства с Windows в Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Често срещани проблеми**

**Разполагам Wi-Fi профил, който зависи от разположени сертификат, посочен в профила за Wi-Fi. Обаче профили за конфигуриране показват състояние на грешка.**

Проверете дали устройството ви е получило сертификата.

1. В Intune отидете на **Всички устройства** и изберете устройството > конфигурация **на устройството**.

2. Проверете дали всички очаквани профили са изброени и в успешно състояние.

3. За профил в Android, ако имате междинни сертификати във вашата верига на сертификати, уверете се, че те са разположени на устройства с Android.

    За да проверите състоянието на сертификата, отидете на **Device Configuration**  >  **Profiles**  >  **Android междинен CA**свойства  >  **Properties**  >  **надежден сертификат**.

Ако продължавате да виждате грешки, прегледайте процедурите и секциите за отстраняване на неизправности. За повече информация вижте [общ преглед за отстраняване на SCEP сертификат профили с Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Разгърнах профил за Wi-Fi към устройство. Intune показва, че е била успешна, но устройството не се свързва с Wi-Fi.**

Успешно състояние означава, че Intune успешно внедри профила като конфигуриран. Тези конфигурации обаче може да не отговарят на изискванията за мрежата и/или удостоверяването. За повече информация относно опит за свързване прегледайте регистрационните файлове в инфраструктурата и услугата за удостоверяване (на Wi-Fi точка за достъп контролер и NPS/Radius сървър). Може да се наложи да работите с екипа по мрежова инфраструктура или доставчика на Wi-Fi на трета страна, за да събирате и преглеждате регистрационни файлове.