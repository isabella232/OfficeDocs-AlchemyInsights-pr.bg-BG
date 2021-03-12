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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708051"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Грешки при синхронизиране поради дублирани обекти

Възможно е да получите едно от следните съобщения за грешка, когато синхронизирането на справочен указател завърши в Microsoft 365:

- Не можете да актуализирате този обект в Microsoft Online Services, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с друг обект в локалния указател.

- Синхронизиран обект със същия адрес за прокси сървър вече съществува във вашия указател на Microsoft Online Services.

- Не можете да актуализирате този обект, тъй като следните атрибути, свързани с този обект, имат стойности, които вече може да са свързани с други обекти във вашите локални справочни услуги: UserPrincipalName.

За да идентифицирате и коригирате проблема, изтеглете и изпълнете [инструмента за отстраняване на грешки в IdFix](https://github.com/Microsoft/idfix).

За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
