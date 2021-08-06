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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998765"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Грешки при синхронизиране поради дублирани обекти

Може да получите едно от следните съобщения за грешка, когато синхронизирането на справочника завърши Microsoft 365:

- Този обект не може да се актуализира в Microsoft Online Services, тъй като следните атрибути, свързани с този обект, имат стойности, които може вече да са свързани с друг обект във вашия локален указател.

- Синхронизиран обект със същия адрес на прокси сървър вече съществува във вашия указател на Microsoft Online Services.

- Този обект не може да се актуализира, тъй като следните атрибути, свързани с този обект, имат стойности, които може вече да са свързани с друг обект във вашите локални справочни услуги: UserPrincipalName.

За да идентифицирате и коригирате проблема, изтеглете и стартирайте инструмента за отстраняване на грешки [idFix DirSync](https://github.com/Microsoft/idfix).

За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
