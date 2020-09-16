---
title: Проблеми с вградените машини
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676871"
---
# <a name="issues-with-onboarding-machines"></a>Проблеми с вградените машини

Възможно е да имате проблеми с вградените машини към услугата MDATP. Ако имате достъп до крайния потребител, изпълнете следните стъпки:

1. Изтеглете диагностичния инструмент за [анализатор на свързването на клиенти](https://aka.ms/mdatpanalyzer) .
2. Extract и Run MDATPAnalyzer. cmd.
3. Намерете диагностичния регистрационен файл в папката, наречена MDATPClientAnalyzerResult, в същата папка, където се изтегля инструментът Analyzer.
4. Прегледайте регистрационния файл MDATPClientAnalyzer.txt, за да намерите проблеми с настройките за свързване или интернет прокси сървъра.