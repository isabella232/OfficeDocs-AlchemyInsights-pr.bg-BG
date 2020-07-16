---
title: За самоличността в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148171"
---
# <a name="about-identity-in-yammer"></a>За самоличността в Yammer

Препоръчва се всички мрежи да предприемат следните стъпки, за да се избегнат свързани с идентичността проблеми:

1. Прилагане на Office 365 самоличност след осигуряване на акаунти в Microsoft 365 за потребители в Azure AD да се гарантира, че всички потребители влизат с помощта на основния си акаунт в Microsoft 365. За повече информация вижте [прилагане на office 365 самоличност за Yammer потребители](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Консолидиране на няколко yammer мрежи. Стари Yammer конфигурации позволяват няколко Yammer мрежи да бъде свързан към един клиент. За повече информация вижте [Миграция на мрежата - консолидиране на множество мрежи Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. По желание на прилагането на лицензиране за Yammer да блокирате потребители от Yammer, ако нямат лиценз. За повече информация вижте [управление на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Накрая проверка на списъка на потребителите за по-стари мрежи на Yammer и спиране на стари потребители. Препоръчва се да преустановите (деактивирате) потребителите, вместо да ги изтривате, защото изтриването е необратимо. За повече информация вижте [Проверка на Yammer потребители в мрежи, свързани към Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) и [премахване на потребители](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Като конфигурирате Yammer чрез тези стъпки, ще бъдете готови да конфигурирате вашата Yammer мрежа за основен режим за Microsoft 365. За повече информация вижте [Конфигуриране на вашата Yammer мрежа за основен режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).