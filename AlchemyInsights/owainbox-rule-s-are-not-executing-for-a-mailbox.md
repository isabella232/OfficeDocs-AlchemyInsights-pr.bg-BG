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
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="521b5-102">На правило за "Входящи" не работи както се очаква</span><span class="sxs-lookup"><span data-stu-id="521b5-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="521b5-103">Проверете следните настройки:</span><span class="sxs-lookup"><span data-stu-id="521b5-103">Verify the following settings:</span></span>

- <span data-ttu-id="521b5-104">Съобщение може да бъдат пренасочени, препращането или отговори автоматично на базата на входящи правила само един път.</span><span class="sxs-lookup"><span data-stu-id="521b5-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="521b5-105">Пренасочване правило (правило за "Входящи" или поща поток правило, известен също като транспортно правило) може да добавите максимум десет спедиция получатели на съобщение.</span><span class="sxs-lookup"><span data-stu-id="521b5-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="521b5-106">За повече информация вижте [дневника, транспорт и входящи правило граници](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="521b5-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="521b5-107">Правилата за "Входящи" не работят на пощенската кутия на алтернативен journaling.</span><span class="sxs-lookup"><span data-stu-id="521b5-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="521b5-108">За повече информация за пощенската кутия на алтернативен journaling вижте [заместник journaling пощенска кутия](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="521b5-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="521b5-109">За да коригирате тези проблеми, вижте [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="521b5-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="521b5-110">Ако предишните въпроси не се прилагат, стартирайте отчета входящи диагностични правило преди да ескалира издаването на поддръжката на Microsoft:</span><span class="sxs-lookup"><span data-stu-id="521b5-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="521b5-111">Отворете пощенската кутия в Outlook в мрежата и щракнете върху **Настройки на** \> **Опции** \> **Организиране имейл** \> **правила на "Входящи"**.</span><span class="sxs-lookup"><span data-stu-id="521b5-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="521b5-112">В дъното на страницата щракнете върху **Ако вашите правила не работят щракнете тук, за да генериране на диагностичен отчет**.</span><span class="sxs-lookup"><span data-stu-id="521b5-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
