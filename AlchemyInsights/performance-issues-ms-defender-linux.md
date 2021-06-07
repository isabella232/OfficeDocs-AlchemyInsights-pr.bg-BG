---
title: Проблеми с производителността за Microsoft Defender за крайна точка на Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793576"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Проблеми с производителността за Microsoft Defender за крайна точка на Linux

Тази статия ви насочва през стъпките за идентифициране на проблеми с производителността за Microsoft Defender за крайна точка на Linux.

Важно е първо да проверите дали проблемът, който срещате, е решен с [най-новата версия](/microsoft-365/security/defender-endpoint/linux-whatsnew). 

За да започнете разследването, вижте Отстраняване [на проблеми с производителността за Microsoft Defender за крайна точка на Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Изключения

Изключенията могат да помогнат за намаляване на проблеми с производителността. Прегледайте изключенията, преди да започнете, така че да се знае и документира допълнителен риск.

За повече информация вижте Конфигуриране [и проверка на изключенията за Microsoft Defender за крайна точка на Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Когато имате няколко файла, & да изключите и всички те са на една и съща точка, може да е по-лесно да изключите точката на монтиране. Започвайки от изданието от февруари 101.22.80, можете да изключите цяла точка.

Ако например /mnt/backup е точка, можете да добавите /mnt/backup към списъка за изключване, като изпълните тази команда:

`$ mdatp exclusion folder add –path /mnt/backup`

**Забележка:** Добавянето на изключения увеличава риска злонамереният софтуер да не бъде откриван и трябва да се обработва и прилага внимателно.

## <a name="need-help"></a>Имате нужда от помощ?

За да ви помогне по най-ефективния начин, съберете диагностичните данни, преди да отворите калъф за поддръжка.
