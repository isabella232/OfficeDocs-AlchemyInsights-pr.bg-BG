---
title: Intune Wi-Fi профили
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028209"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi профили

Успешното внедряване на Wi-Fi за клиенти на MDM зависи от правилно разположен профил, който отразява изискванията на корпоративната Wi-Fi инфраструктура. За да прегледате подходящите настройки за клиентските платформи, които проучвате, вижте: 

[Добавяне Wi-Fi настройки за устройства с Android в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Добавяне Wi-Fi за устройства с Android Enterprise, специализирани и напълно управлявани в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Добавяне Wi-Fi настройки за устройства с iOS и iPadOS в Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Добавяне Wi-Fi настройки за Windows 10 по-нови устройства в Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Импортиране Wi-Fi настройки за Windows устройства в Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Често срещани проблеми**

**Разполагам профил на Wi-Fi, който е зависим от разположил се сертификат, зададен в Wi-Fi профил. Обаче профилите за конфигуриране показват състояние на грешка.**

Проверете дали устройството ви е получило сертификата.

1. В Intune отидете на **Всички устройства и** изберете устройството > **конфигурацията на устройството**.

2. Проверете дали всички очаквани профили са изброени и в успешно състояние.

3. За профил на Android, ако имате междинни сертификати във вашата верига от сертификати, уверете се, че те са разположени на устройства с Android.

    За да проверите състоянието на сертификата, отидете на **Профили за конфигуриране** на устройства с  >  **надежден** сертификат за междинни CA свойства  >    >    >  **на** Android.

Ако продължите да виждате грешки, прегледайте разделите за процедури и отстраняване на неизправности. За повече информация вижте Общ преглед за отстраняване на неизправности с профилите на [SCEP сертификати с Microsoft Intune.](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

**Разположих Wi-Fi профил на устройство. Intune показва, че е успешно, но устройството не се свързва към Wi-Fi.**

Успешното състояние означава, че Intune успешно е разположил профила като конфигуриран. Тези конфигурации обаче може да не отговарят на изискванията за вашата мрежа и/или удостоверяване. За повече подробности относно опитната връзка прегледайте регистрационните файлове в услугата за инфраструктура и удостоверяване (на Wi-Fi access point controller и NPS/Radius сървър). Може да се наложи да работите с екипа за мрежова инфраструктура или с доставчика на Wi-Fi, за да събирате и преглеждате регистрационни файлове.