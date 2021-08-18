---
title: Грешка за DLP лицензиране на крайна точка
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200001"
- "7176"
ms.openlocfilehash: c32ab88a72c265be411350e50756f5b2e1e3337c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322120"
---
# <a name="endpoint-dlp-licensing-error"></a>Грешка "DLP лицензиране на крайна точка"

Когато се опитвате да настроите Endpoint DLP, ако получите следната грешка:

`Your organization is missing the licenses required to manage these devices`.

Уверете се, че имате един от следните абонаменти или добавки:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Microsoft 365 E5 съответствие
- Microsoft 365 A5 съответствие
- Microsoft 365 E5 на информацията и управлението
- Microsoft 365 A5 на информацията и управлението

**Забележка:** Това няма да работи за комбинации от лицензи като: Win E5 + O365 E5 + EMS E5. Трябва да имате чист лиценз за M365 E5, за да настроите тази функция.

За повече информация за DLP лицензирането на Крайна точка вижте [Лицензиране на DLP за крайна точка.](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)
