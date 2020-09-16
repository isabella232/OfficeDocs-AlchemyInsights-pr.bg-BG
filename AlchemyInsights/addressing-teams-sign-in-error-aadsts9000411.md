---
title: Отстраняване на грешки при влизане в AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 8ca3793b8cd12b7ad2510ca0b3be58c32a61c14c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47687027"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>Отстраняване на грешки при влизане в AADSTS9000411

Когато влизате в Microsoft Teams, е възможно да получите грешката: **Съжаляваме, но имаме проблеми с влизането ви в AADSTS9000411: заявката не е правилно форматирана. Параметърът "login_hint" е дублиран.**

За да адресирате този проблем, уверете се, че вашите клиенти на Microsoft Teams се актуализират. За повече информация за актуализирането на клиента вижте [актуализиране на Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

Ако не можете да актуализирате своя клиент по някаква причина, излизането от клиента ще изчисти повечето кеширани данни. Ако обаче все още имате проблеми след излизане/влизане, излезте от Teams и моля, изчистете кеша на клиента си, като направите следното:
1. Затворете Microsoft Teams.
2. Отидете на:%AppData%\microsoft\teams и изтрийте всички файлове.
3. Отворете повторно Microsoft Teams.
