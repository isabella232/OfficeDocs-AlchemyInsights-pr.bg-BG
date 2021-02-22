---
title: Скриване на публични папки
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315313"
---
# <a name="hide-public-folders"></a>Скриване на публични папки

**За да скриете цялото дърво на публичната папка**:

Използвайте стъпките в [тази](https://aka.ms/ControlPF) статия, за да скриете цялото дърво на публичната папка от селективни или всички потребители.

**За да скриете конкретна публична папка**:

1. Добавяне на разрешения за потребителите, които се нуждаят от достъп до публичната папка

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Отстранете потребителя **по подразбиране** от списъка с **разрешения** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
