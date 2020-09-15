---
title: Отстраняване на неизправности с пояснението за безопасността за проверки за откриване на измами
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658399"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Отстраняване на неизправности с пояснението за безопасността за проверки за откриване на измами

Ако получавате съвет за безопасност, който гласи "подателят е провалил нашите проверки за откриване на измами и може да не е този, който изглежда, че е", тогава подателят не е успял да премине или проверки за удостоверяване на DKIM или SPF. Най-добрият метод за разрешаване на това е подателят да се оторизира. Ако подателят е изпратил от ваше име, трябва да го упълномощите, като добавите IP адреса на подателя към своя SPF запис.
  
Вижте [отстраняване на проблеми с червения (подозрителен) съвет за безопасност за проверка](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) за повече информация.
  
Ето някои други връзки, които могат да ви помогнат:
  
- [Как Microsoft използва рамката за правилата на подателя (SPF), за да предотврати фалшифициране](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настройване на SPF за предотвратяване на фалшифицирането](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
