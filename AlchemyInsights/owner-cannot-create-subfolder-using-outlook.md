---
title: Собственикът не може да създава подпапка с помощта на Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063113"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Собственикът не може да създава подпапка с помощта на Outlook

**Има текущ проблем със собствениците на публични папки, които създават подпапки чрез Outlook. Проблемът скоро ще бъде коригиран.**

Междувременно използвайте едно от следните заобиколни решения:

1. Използвайте Outlook mac, за да създадете подпапка, тъй като проблемът засяга само Outlook за настолни прозорци (всички версии)
2. Дайте на администратора да създаде подпапката с помощта на EXO Shell или EAC
3. Промяна на папката DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя на други пощенски кутии, различни от пощенската кутия за съдържание за папката, която причинява проблем  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Изчакайте един час, рестартирайте клиента на Outlook