---
title: Отдалечено отстраняване на проблеми при внедряване на устройства с Windows 10 за защита от защитата на Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692557"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Отдалечено отстраняване на проблеми при внедряване на устройства с Windows 10 за защита от защитата на Microsoft Defender

Ако имате достъп до отдалечения компютър, изпълнете следните стъпки:

1. Изтеглете диагностичния инструмент за [анализатор на свързването на клиенти](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Extract и Run MDATPAnalyzer. cmd.
3. Намерете диагностичния регистрационен файл в папката MDATPClientAnalyzerResult, която е същата папка, в която е изтеглен инструментът Analyzer.
4. За да намерите проблеми с настройките за свързване или интернет прокси сървъра, Прегледайте регистрационния файл MDATPClientAnalyzer.txt.

За да научите повече, вижте [проблеми с вградените машини](https://go.microsoft.com/fwlink/?linkid=2143634).
