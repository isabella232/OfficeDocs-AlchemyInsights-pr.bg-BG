---
title: Отстраняване на неизправности с съвета за безопасност за проверки за откриване на измами
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834720"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Отстраняване на неизправности с съвета за безопасност за проверки за откриване на измами

Ако получавате съвет за безопасност, който гласи "Подателят не е изпълнил нашите проверки за откриване на измами и може да не е този, който изглежда, че е", тогава подателят не е преминал проверки за удостоверяване на DKIM или SPF. Най-добрият метод за разрешаване на проблема е подателят да се оторизира. Ако подателят изпраща от ваше име, трябва да го оторизирате, като добавите IP адреса на подателя към вашия SPF запис.
  
Вижте [Отстраняване на неизправности с червения (подозрителен) съвет за безопасност за проверки за откриване на](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) измами за повече информация.
  
Ето някои други връзки, които могат да ви помогнат:
  
- [Как Microsoft използва рамката за правила за податели (SPF), за да предотврати подсказка](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настройване на SPF за предотвратяване на подпухване](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
