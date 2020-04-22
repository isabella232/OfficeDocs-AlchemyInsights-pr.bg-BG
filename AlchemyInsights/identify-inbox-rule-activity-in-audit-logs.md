---
title: Идентифицирайте входящата дейност в регистрационните файлове за проверка
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716413"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="e5663-102">Идентифицирайте входящата дейност в регистрационните файлове за проверка</span><span class="sxs-lookup"><span data-stu-id="e5663-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="e5663-103">Можете да използвате проверка регистър търсене в Microsoft 365 Security & съответствие център за преглед на събития във входящата кутия (създаване, промяна и изтриване на правила за входящата поща).</span><span class="sxs-lookup"><span data-stu-id="e5663-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="e5663-104">Влезте в центъра за сигурност на [Microsoft 365 & съответствие .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="e5663-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e5663-105">Отидете на страницата **за** > **търсене на регистрационния файл за проверка.**</span><span class="sxs-lookup"><span data-stu-id="e5663-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e5663-106">Изберете периода от време в полетата **Начална дата** и **Крайна дата.**</span><span class="sxs-lookup"><span data-stu-id="e5663-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="e5663-107">Под **Дейности на пощенската кутия**на Exchange проверете полето **дейности** е настроен на **Създаване/модифициране/модифициране/разрешаване/забраняване**на правило за пощенска кутия .</span><span class="sxs-lookup"><span data-stu-id="e5663-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="e5663-108">Щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="e5663-108">Click **Search**.</span></span>

<span data-ttu-id="e5663-109">В резултатите изберете запис за проверка.</span><span class="sxs-lookup"><span data-stu-id="e5663-109">In the results, select an audit record.</span></span> <span data-ttu-id="e5663-110">В допълнителното меню за подробни данни щракнете върху **Още информация**.</span><span class="sxs-lookup"><span data-stu-id="e5663-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="e5663-111">Информация за настройките на правилото за входяща тава се показва в полето **параметри** .</span><span class="sxs-lookup"><span data-stu-id="e5663-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="e5663-112">За повече информация вижте [Определяне дали потребителят създава правило за входяща поща](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="e5663-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
