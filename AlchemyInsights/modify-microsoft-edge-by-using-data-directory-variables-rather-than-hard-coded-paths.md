---
title: Променете Microsoft Edge с помощта на променливите на указателя на данни, а не на трудни кодирани пътища
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034879"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>Променете Microsoft Edge с помощта на променливите на указателя на данни, а не на трудни кодирани пътища

Например в Windows, за да съхраните профилните данни под локалните данни на потребителя, а не в местоположението по подразбиране, задайте правилата за *UserDataDir* на **$ {local_app_data} \Edge\Profile**.

За повече информация вижте [Създаване на променливи на директорията на потребителските данни за Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-policies).