---
title: Идентифициране на входящи правило дейност в регистрационните файлове от одита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755027"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="489ae-102">Идентифициране на входящи правило дейност в регистрационните файлове от одита</span><span class="sxs-lookup"><span data-stu-id="489ae-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="489ae-103">Можете да използвате одит регистрационния файл търсене в защита & съответствие център да видите входящи правило събития (създаване, модифициране и изтриване на правила за входяща поща).</span><span class="sxs-lookup"><span data-stu-id="489ae-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="489ae-104">Влезте в [Office 365 сигурност & съответствие център](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="489ae-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="489ae-105">Щракнете върху **търсене и проучване** и изберете **Одит регистрационния файл търсене**.</span><span class="sxs-lookup"><span data-stu-id="489ae-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="489ae-106">Изберете диапазона от дати в полетата **Начална дата** и **крайна дата** .</span><span class="sxs-lookup"><span data-stu-id="489ae-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="489ae-107">Под **Exchange пощенска кутия дейности**проверете полето **дейности** е зададена на **Ню-InboxRule създаване/промяна/разрешаване/забраняване на правило за "Входящи"**.</span><span class="sxs-lookup"><span data-stu-id="489ae-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="489ae-108">Щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="489ae-108">Click **Search**.</span></span>

<span data-ttu-id="489ae-109">В резултатите изберете отчет.</span><span class="sxs-lookup"><span data-stu-id="489ae-109">In the results, select an audit record.</span></span> <span data-ttu-id="489ae-110">В детайли flyout щракнете върху **Повече информация**.</span><span class="sxs-lookup"><span data-stu-id="489ae-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="489ae-111">Информация за настройките на правило за "Входящи" се показва в полето за **параметри** .</span><span class="sxs-lookup"><span data-stu-id="489ae-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="489ae-112">За повече информация вижте [определя, ако потребителят създаде правило за "Входящи"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="489ae-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
