---
title: Конфигуриране на услугата за домейни
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884863"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Не можете да разрешите използването на пад-DS или разполагане е неуспешно

За да се реши проблемът с услугата за домейни на Azure AD (пад-DS), която не е разрешена или не може да бъде разгърната, изпълнете следните стъпки:

1. Ако използвате вече съществуваща виртуална мрежа, проверете своя ГЯД за правила, които блокират портове, необходими за синхронизиране в пад-DS в портала https://aka.ms/aadds-networking .
2. Проверете дали за съобщението за грешка е отговорено в това ръководство за отстраняване на неизправности, което е налично в  https://aka.ms/aadds-troubleshoot-enable .
3. Опитайте да разположите услугите за домейни на Azure AD в нова виртуална мрежа.
4. Следвайте ръководството "Начално запознаване" как да разположите пад-DS: [Създаване и конфигуриране на услуги за домейни на пад](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ако имате проблеми с разполагането на Azure AD Domain Services, вижте [отстраняване на неизправности в AZURE ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) за разрешаване на често срещани грешки, които да ви помогнат да работите отново. 

**Не можете да забраните пад-DS**

ПАД-ДС не може да бъде спрян. Ако искате да спрете да използвате своя управляван домейн, той трябва да бъде изтрит.
За да изтриете управлявания домейн, вижте [Изтриване на услуга за домейн на пад](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



