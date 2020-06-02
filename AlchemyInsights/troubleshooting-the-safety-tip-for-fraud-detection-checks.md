---
title: Отстраняване на неизправности на върха за безопасност при проверки за откриване на измами
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504972"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>Отстраняване на неизправности на върха за безопасност при проверки за откриване на измами

Ако получавате съвет за безопасност, който казва "Подателят не успя да ни проверява за откриване на измами и може да не е кой да изглежда те", след това подателят не успя да премине или DKIM или SPF удостоверяване проверки. Най-добрият начин за разрешаване на проблема е подателят да се упълномощава. Ако изпращачът изпраща от ваше име, трябва да го упълномощите, като добавите IP адреса на подателя към вашия SPF запис.
  
Вижте [Отстраняване на неизправности с червения (подозрителен) съвет за безопасност за проверки](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) за откриване на измами за повече информация.
  
Ето някои други връзки, които могат да помогнат:
  
- [Как Microsoft използва правилата за подателя (SPF) за предотвратяване на подправяне](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [Настройте SPF, за да предотвратите подправяне](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
