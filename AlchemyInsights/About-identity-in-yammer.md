---
title: За самоличността в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664159"
---
# <a name="about-identity-in-yammer"></a>За самоличността в Yammer

Препоръчва се всички мрежи да предприемат следните стъпки, за да се избегнат проблеми, свързани с самоличността:

1. Използвайте самоличността на Office 365, след като осигурите акаунтите за Microsoft 365 за потребители в Azure AD, за да сте сигурни, че всички потребители ще влизат, като използват основния си акаунт за Microsoft 365. За повече информация вижте [прилагане на самоличността на Office 365 за потребители на Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Консолидиране на няколко мрежи Yammer. Наследени конфигурации на Yammer разрешават много мрежи на Yammer да бъдат свързани с един клиент. За повече информация вижте [мрежа за мигриране – консолидиране на няколко мрежи Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Ако желаете, можете да наложите лицензиране за Yammer, за да блокирате потребители от Yammer, ако нямат лиценз. За повече информация вижте [управление на потребителските лицензи за Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. И накрая, Претърсете списъка с потребители за по-стари мрежи на Yammer и преустановявайте наследени потребители. Препоръчително е да прекратите (дезактивирате) потребители, вместо да ги изтривате, тъй като изтриването е необратимо. За повече информация вижте [проверка на потребителите на Yammer в мрежите, свързани с Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) , и [Премахване на потребители](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Чрез конфигуриране на Yammer с помощта на тези стъпки ще можете също да конфигурирате своята мрежа на Yammer за основен режим за Microsoft 365. За повече информация вижте [Конфигуриране на вашата мрежа на Yammer за роден режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).