---
title: Адресиране на грешка при влизане в Teams AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821976"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Адресиране на грешка при влизане в Teams AADSTS9000411

Когато влезете в Microsoft Teams, може да получите грешката: За съжаление, имаме проблеми с влизането ви в **AADSTS9000411: Искането не е форматирано правилно. Параметърът "login_hint" е дублиран.**

За да решите този проблем, уверете се, че вашите клиенти на Microsoft Teams са актуализирани. За повече информация относно актуализирането на вашия клиент вижте [Актуализиране на Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ако по някаква причина не можете да актуализирате клиента си, излизането от клиента ще изчисти повечето кеширани данни. Ако обаче все още имате проблеми след излизане/влизане, излезте от Teams и изчистете кеша на клиента, като направите следното:
1. Затворете Microsoft Teams.
2. Отидете на: %appdata%\microsoft\teams и изтрийте всички файлове.
3. Отворете отново Microsoft Teams.
