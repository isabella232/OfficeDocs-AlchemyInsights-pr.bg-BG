---
title: 1332 OWA - входящи правило(а) са не изпълнение за пощенска кутия
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372549"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>На правило за "Входящи" не работи както се очаква

Проверете следните настройки:

- Съобщение може да бъдат пренасочени, препращането или отговори автоматично на базата на входящи правила само един път. Пренасочване правило (правило за "Входящи" или поща поток правило, известен също като транспортно правило) може да добавите максимум десет спедиция получатели на съобщение. За повече информация вижте [дневника, транспорт и входящи правило граници](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правилата за "Входящи" не работят на пощенската кутия на алтернативен journaling. За повече информация за пощенската кутия на алтернативен journaling вижте [заместник journaling пощенска кутия](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

За да коригирате тези проблеми, вижте [KB 2829319](https://support.microsoft.com/kb/2829319).

Ако предишните въпроси не се прилагат, стартирайте отчета входящи диагностични правило преди да ескалира издаването на поддръжката на Microsoft:

1. Отворете пощенската кутия в Outlook в мрежата и щракнете върху **Настройки на** \> **Опции** \> **Организиране имейл** \> **правила на "Входящи"**.

2. В дъното на страницата щракнете върху **Ако вашите правила не работят щракнете тук, за да генериране на диагностичен отчет**.
