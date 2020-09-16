---
title: 902 (грешки при синхронизиране поради дублирани обекти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737330"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Грешки при синхронизиране поради дублирани обекти

Възможно е да получите едно от следните съобщения за грешка, когато синхронизирането на справочен указател завърши в Microsoft 365:

- Не можете да актуализирате този обект в Microsoft Online Services, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с друг обект в локалния указател.

- Синхронизиран обект със същия адрес за прокси сървър вече съществува във вашия указател на Microsoft Online Services.

- Не можете да актуализирате този обект, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с други обекти във вашите локални справочни услуги: UserPrincipalName.

За да идентифицирате и коригирате проблема, изтеглете и изпълнете [инструмента за отстраняване на грешки в IdFix](https://www.microsoft.com/download/details.aspx?id=36832).

За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
