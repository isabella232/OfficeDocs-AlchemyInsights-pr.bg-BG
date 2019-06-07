---
title: 902 (синхронизиране грешки поради дублиращи обекти)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757984"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Грешките при синхронизиране поради дублиращи се обекти

Може да се появи едно от следните съобщения за грешка при синхронизиране на директории завършва:

- Не може да актуализира този обект в онлайн услугите на Microsoft, защото следните атрибути, свързани с този обект имат стойности, които вече са свързани с друг обект в местна директория.

- Синхронизиран обект със същия прокси адрес вече съществува в директорията си онлайн услугите на Microsoft.

- Не може да актуализира този обект, защото следните атрибути, свързани с този обект имат стойности, които вече са свързани с друг обект в вашата местен справочни услуги: UserPrincipalName.

За да идентифицирате и отстраните проблема, изтеглете и изпълнете [IdFix DirSync грешка отстраняване инструмент](https://www.microsoft.com/download/details.aspx?id=36832).

За повече информация вижте [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
