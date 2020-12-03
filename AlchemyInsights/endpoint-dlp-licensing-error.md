---
title: Грешка на DLP за лицензиране на крайна точка
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
ms.openlocfilehash: d17c51177898d62c7c477460c8c26b4753bae65f
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564384"
---
# <a name="endpoint-dlp-licensing-error"></a>Грешка на DLP за лицензиране на крайна точка

Когато се опитвате да настроите точка DLP, ако получите следната грешка:

`Your organization is missing the licenses required to manage these devices`.

Уверете се, че имате един от следните абонаменти или добавки:

- Microsoft 365 E5
- Microsoft 365 A5 (EDU)
- Съответствие на Microsoft 365 E5
- Съответствие на Microsoft 365 A5
- Microsoft 365 E5 Protection и управление на информацията
- Защита и управление на информацията за Microsoft 365 A5

> [!NOTE]
> Това няма да работи за комбинации от лицензи, като например: Win E5 + O365 E5 + EMS E5. Трябва да имате чист лиценз за M365 E5, за да настроите тази функция.

За повече информация за характеристиките на DLP за лицензиране вижте " [крайна точка](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management) за лицензиране"
