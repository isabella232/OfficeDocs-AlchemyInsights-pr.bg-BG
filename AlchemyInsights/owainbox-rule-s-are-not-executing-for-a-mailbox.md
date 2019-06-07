---
title: 1332 OWA - входящи правило(а) са не изпълнение за пощенска кутия
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762212"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>На правило за "Входящи" не работи както се очаква

Проверете следните настройки:

- Съобщение може да бъдат пренасочени, препращането или отговори автоматично на базата на входящи правила само един път. Пренасочване правило (правило за "Входящи" или поща поток правило, известен също като транспортно правило) може да добавите максимум десет спедиция получатели на съобщение. За повече информация вижте [дневника, транспорт и входящи правило граници](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правилата за "Входящи" не работят на пощенската кутия на алтернативен journaling. За повече информация за пощенската кутия на алтернативен journaling вижте [заместник journaling пощенска кутия](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

За да коригирате тези проблеми, вижте [KB 2829319](https://support.microsoft.com/kb/2829319).

Ако предишните въпроси не се прилагат, стартирайте отчета входящи диагностични правило преди да ескалира издаването на поддръжката на Microsoft:

1. Отворете пощенската кутия в Outlook в мрежата и щракнете върху **Настройки на** \> **Опции** \> **Организиране имейл** \> **правила на "Входящи"**.

2. В дъното на страницата щракнете върху **Ако вашите правила не работят щракнете тук, за да генериране на диагностичен отчет**.
