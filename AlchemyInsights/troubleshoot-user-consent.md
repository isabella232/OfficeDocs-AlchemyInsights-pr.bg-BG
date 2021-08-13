---
title: Отстраняване на неизправности с съгласието на потребителя
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007887"
---
# <a name="troubleshoot-user-consent"></a>Отстраняване на неизправности с съгласието на потребителя

1. Можете да конфигурирате как крайните потребители да се съгласяват с приложенията чрез портала на Azure или PowerShell. Вижте [Настройки за съгласие на потребителя](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) за повече информация.
1. Администраторът може също да използва [API Graph Microsoft,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) за да даде съгласие за делегирани разрешения от името на един потребител. За повече информация вижте [Получаване на достъп от името на потребител](https://docs.microsoft.com/graph/auth-v2-user).
1. [Грешки при съгласието на](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)потребителя: в тази статия се обсъждат грешките, които могат да възникнат по време на процеса на съгласие с дадено приложение. Ако отстранявате неочаквани подкани за съгласие, които не съдържат съобщения за грешка, вижте [Сценарии за удостоверяване за Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).