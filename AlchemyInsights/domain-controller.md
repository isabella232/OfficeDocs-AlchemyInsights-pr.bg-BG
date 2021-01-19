---
title: Домейнов контролер
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900762"
---
# <a name="domain-controller"></a>Домейнов контролер

**Не можете да разрешите използването на пад-DS или разполагане е неуспешно**

За да се реши проблемът с услугата за домейни на Azure AD (пад-DS), която не е разрешена или не може да бъде разгърната, изпълнете следните стъпки:

1. Ако използвате вече съществуваща виртуална мрежа, проверете своя ГЯД за правила, които блокират портове, необходими за синхронизиране в пад-DS в портала https://aka.ms/aadds-networking .
2. Проверете дали за съобщението за грешка е отговорено в това ръководство за отстраняване на неизправности, което е налично в  https://aka.ms/aadds-troubleshoot-enable .
3. Опитайте да разположите услугите за домейни на Azure AD в нова виртуална мрежа.
4. Следвайте ръководството "Начално запознаване" как да разположите пад-DS, което е налично в [ръководството, за да създадете AZURE ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Ако имате проблеми с разполагането на Azure AD Domain Services, вижте [отстраняване на неизправности в AZURE ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) за разрешаване на често срещани грешки, които да ви помогнат да работите отново. 

**Не можете да забраните пад-DS**

ПАД-ДС не може да бъде спрян. Ако искате да спрете да използвате своя управляван домейн, той трябва да бъде изтрит.

Ако срещнете проблеми, за да решите често срещани съобщения за грешка и за свързани стъпки за отстраняване на неизправности, за да ви помогнат да започнете да работите отново, вижте [отстраняване на неизправности в Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
