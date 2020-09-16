---
title: Собственик не може да създаде подпапка с помощта на Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665707"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Собственик не може да създаде подпапка с помощта на Outlook

**Има текущ проблем с собственици на публични папки, създаващи подпапки с помощта на Outlook. Проблемът ще бъде коригиран скоро.**

Междувременно Използвайте едно от следните заобиколни решения:

1. Използвайте Outlook for MAC, за да създадете подпапката, тъй като проблемът влияе само на Outlook за настолната версия на Windows (всички версии)
2. Помолете администратор да създаде подпапката, като използва ЕКСО черупка или EAC
3. Промяна на DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя в друга пощенска кутия от пощенската кутия на съдържанието за папката, която създава проблема  
    - *Set-пощенска кутия user1 DefaultPublicFolderMailbox PubMBX3*
4. Изчакайте един час, рестартирайте клиент на Outlook