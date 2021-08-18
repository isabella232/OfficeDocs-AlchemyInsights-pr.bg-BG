---
title: Изпращане на известия по избор с Intune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086153"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>Как да изпращате известия по избор до потребителите на управлявани устройства с iOS и Android

Известията по избор за Intune се обработват от Company Portal на устройството на потребителя. След това приложението създава push известието на това устройство.

По-долу са необходими предпоставки за устройството, за да се поддържа получаването на известия по избор, а приложението след това да създаде push известието:

- Устройството трябва да има инсталирано Company Portal приложение.  

- Устройството трябва да позволи на Company Portal да изпраща push известия. Когато приложението е инсталирано или актуализирано, то ще подкани потребителя да разреши известията.

- Устройствата с Android трябва да имат инсталирани услуги на Google Play.

- Устройството трябва да бъде записано в Intune.

За повече информация, включително как да изпратите съобщение, вижте документацията [за функциите](https://docs.microsoft.com/intune/custom-notifications).
