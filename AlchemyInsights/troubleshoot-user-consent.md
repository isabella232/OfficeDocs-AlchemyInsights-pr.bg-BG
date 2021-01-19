---
title: Отстраняване на проблеми с потребителското съгласие
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
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900838"
---
# <a name="troubleshoot-user-consent"></a>Отстраняване на проблеми с потребителското съгласие

1. Можете да конфигурирате как крайните потребители да се съгласяват с приложения през портала на Azure или PowerShell. Вижте [Настройки на потребителско съгласие](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) за повече информация.
1. Администраторът може също да използва [API за Microsoft Graph](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , за да даде съгласие за делегираните разрешения от името на един потребител. За повече информация вижте [получаване на достъп от името на потребител](https://docs.microsoft.com/graph/auth-v2-user).
1. [Грешки при одобрение на потребители](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): тази статия описва грешки, които могат да възникнат по време на процеса на даване на съгласие на приложение. Ако отстранявате проблеми с неочакваното съгласие, които не съдържат съобщения за грешка, вижте [сценарии за удостоверяване за AZURE ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).