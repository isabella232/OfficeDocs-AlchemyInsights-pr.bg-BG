---
title: 1332 OWA – правилото(ята) за папка "Входящи" не се изпълняват за пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040891"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило за папка "Входящи" не работи според очакванията

Проверете следните настройки в Outlook в уеб:

- Съобщението може да бъде пренасочено, препратено или отвърнато на автоматично въз основа на правилата за папка "Входящи" само веднъж. Правило за пренасочване (правило за папка "Входящи" или правило за пощенски поток, известно още като транспортно правило), може да добави максимум десет получатели за препращане към съобщение. За повече информация вижте Ограничения [за правилото "Дневник", "Транспорт" и "Входящи".](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Правилата за папка "Входящи" не работят в алтернативната пощенска кутия за дневници. За повече информация относно алтернативната пощенска кутия за дневници вж. [Алтернативна пощенска кутия за дневници.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

За да коригирате тези проблеми, [вижте Kb 2829319](https://support.microsoft.com/kb/2829319).

Ако предишните проблеми не важат, изпълнете диагностичния отчет за правилото "Входящи", преди да ескалирате проблема към поддръжката от Microsoft:

1. Отворете пощенската кутия в Outlook в уеб и щракнете върху <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Настройки**  >  **Преглед на всички Outlook Настройки**  >  **Поща**  >  **Правила**.

2. В долната част на страницата щракнете върху Ако правилата ви не работят, **щракнете тук, за да генерирате диагностичен отчет**.
