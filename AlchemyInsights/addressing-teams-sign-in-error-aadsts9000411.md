---
title: Адресиране Teams при влизане AADSTS9000411
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
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952999"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Адресиране Teams при влизане AADSTS9000411

Когато влезете в Microsoft Teams, може да получите грешката: За съжаление, но имаме проблеми с влизането ви в **AADSTS9000411: Заявката не е форматирана правилно. Параметърът "login_hint" е дублиран.**

За да решите този проблем, уверете се, че вашите Microsoft Teams клиенти се актуализират. За повече информация относно актуализирането на вашия клиент вижте [Актуализиране Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ако по някаква причина не можете да актуализирате клиента си, излизането от клиента ще изчисти повечето кеширани данни. Ако обаче все още имате проблеми след излизане/влизане, затворете Teams и изчистете кеша на клиента, като направите следното:
1. Затворете Microsoft Teams.
2. Отидете на: %appdata%\microsoft\teams и изтрийте всички файлове.
3. Отворете отново Microsoft Teams.
