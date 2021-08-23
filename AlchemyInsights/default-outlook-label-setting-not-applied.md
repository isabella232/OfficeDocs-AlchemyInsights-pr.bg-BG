---
title: Настройката Outlook етикет по подразбиране не е приложена
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454436"
---
# <a name="default-outlook-label-setting-not-applied"></a>Настройката Outlook етикет по подразбиране не е приложена

Ако настройките на Outlook по подразбиране за етикети не се прилагат правилно и се приложи друг етикет или не е приложен етикет, може да имате известен проблем (MC277818) и трябва да направите някоя от тези 2 опции, за да отстраните проблема:

**Опция 1:**

1. Отидете в центъра Microsoft 365 за съответствие > **решения за защита** на  >  **информацията**.
1. Изберете **Правила за етикети** и изберете правилата за етикети, които трябва да редактирате (**настройката на OutlookDefaultlabel** не е зададена правилно във въпросните правила за етикети. Изпълнете **Get-labelpolicy, за** да видите тази настройка), и след това изберете **Редактиране на правила**.
1. Изберете **Напред,** докато не видите настройката Прилагане на този етикет по подразбиране към имейли **,** която е налична, ако изберете Изисквай от потребителите да прилагат етикет към имейли **и** документи на наследник в диалоговия **прозорец Настройки** на правила.
1. В диалоговия **прозорец Прилагане на етикет по** подразбиране към документи изберете **Няма** от падащия списък.
1. Изберете **Напред и** **Подай, за** да запишете настройките на етикета.

**Опция 2:**

В [Центъра за защита и съответствие Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)използвайте командата Set-LabelPolicy, за да промените **OutlookDefaultlabel** на **Няма** в {OutlookDefaultLabel="None"}.

Изпълнение: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

За повече информация относно етикетите по подразбиране за Outlook вижте [Задаване на друг етикет по подразбиране за Outlook.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook)