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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918926"
---
# <a name="about-identity-in-yammer"></a>За самоличността в Yammer

Препоръчително е всички мрежи да предприемат следните стъпки, за да избегнат проблеми, свързани с самоличността:

1. Налагане Office 365 самоличност след осигуряването на Microsoft 365 акаунти за потребители в Azure AD, за да се гарантира, че всички потребители ще впишат, като използват своя основен Microsoft 365 акаунт. За повече информация вижте Налагане [на Office 365 за Yammer потребители](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Консолидиране на няколко Yammer мрежи. Наследените Yammer позволяват няколко Yammer да бъдат свързани към един клиент. За повече информация вижте [Мигриране на мрежата – Консолидиране на няколко Yammer мрежи](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Ако желаете, наложат лицензиране за Yammer да блокират потребителите от Yammer, ако нямат лиценз. За повече информация вижте Управление [на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. И накрая, проверявайте потребителския списък за по-стари Yammer мрежи и преустановявате наследените потребители. Препоръчително е да преустановите (дезактивирате) потребителите, вместо да ги изтривате, тъй като изтриването е необратимо. За повече информация вижте Проверка [на Yammer потребители в мрежи, свързани с Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) и Премахване на [потребители](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Като конфигурирате Yammer тези стъпки, ще бъдете готови да конфигурирате вашата Yammer мрежа за основен режим за Microsoft 365. За повече информация вижте Конфигуриране [на вашата Yammer за основен режим за Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)