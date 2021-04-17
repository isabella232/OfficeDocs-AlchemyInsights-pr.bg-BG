---
title: Собственикът не може да създаде подпапка с помощта на Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836124"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Собственикът не може да създаде подпапка с помощта на Outlook

**Има текущ проблем със собствениците на публични папки, които създават подпапки с помощта на Outlook. Проблемът скоро ще бъде коригиран.**

Междувременно използвайте едно от следните заобиколни решения:

1. Използвайте Outlook for MAC, за да създадете подпапка, тъй като проблемът засяга само Outlook за настолни прозорци (всички версии)
2. Дайте на администратора да създаде подпапката с помощта на EXO Shell или EAC
3. Промяна на папката DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя на други пощенски кутии, различни от пощенската кутия за съдържание за папката, която причинява проблем  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Изчакайте един час, рестартирайте клиента на Outlook