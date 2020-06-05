---
title: 1332 OWA - входящи правила не се изпълняват за пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576549"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило за входяща поща не работи според очакванията

Проверете следните настройки в Outlook в мрежата:

- Едно съобщение може да бъде пренасочено, препратено или да се отговаря автоматично на базата на правила за входяща поща само веднъж. Пренасочващо правило (правило за входящи съобщения или правило за пощенски поток, известно също като транспортно правило) може да добави до десет адресата на препращане към съобщение. За повече информация вижте [журнал, транспорт и входящи правила ограничава](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правилата за входящи не работят в пощенската кутия за алтернативен журнал. За повече информация относно пощенска кутия за алтернативен журнали вижте [пощенска кутия за алтернативни дневници](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

За да решите тези проблеми, вижте [KB 2829319](https://support.microsoft.com/kb/2829319).

Ако предишните проблеми не се прилагат, изпълнете inbox правило диагностичен отчет преди да ескалира проблема за поддръжка на Microsoft:

1. Отворете пощенската кутия в Outlook в мрежата и щракнете върху <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Настройки на настройките**  >  **Преглед на всички настройки на**  >  Outlook **Поща**  >  **Правила за**

2. В долната част на страницата щракнете върху **Ако вашите правила не работят, щракнете тук, за да генерирате диагностичен отчет**.
