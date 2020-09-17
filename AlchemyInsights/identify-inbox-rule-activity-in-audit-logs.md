---
title: Идентифициране на дейността с правила за папка "Входящи" в регистрационни файлове за проверка
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779040"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="003e1-102">Идентифициране на дейността с правила за папка "Входящи" в регистрационни файлове за проверка</span><span class="sxs-lookup"><span data-stu-id="003e1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="003e1-103">Можете да използвате функцията за търсене в регистрационния файл за проверка в центъра за защита на & на Microsoft 365, за да преглеждате събития за правилата за входящи (създаване, модифициране и изтриване на правила за входящи).</span><span class="sxs-lookup"><span data-stu-id="003e1-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="003e1-104">Влезте в центъра за [съответствие на & на Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="003e1-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="003e1-105">Отидете на страницата **Search**за  >  **търсене в регистрационния файл за проверка** на търсенето.</span><span class="sxs-lookup"><span data-stu-id="003e1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="003e1-106">Изберете диапазона от дати в полетата " **Начална дата** " и " **крайна дата** ".</span><span class="sxs-lookup"><span data-stu-id="003e1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="003e1-107">Под **дейности за пощенска кутия на Exchange**Проверете дали полето **дейности** е зададено на " **InboxRule" Създаване/промяна/разрешаване/забраняване на правило за папка "Входящи"**.</span><span class="sxs-lookup"><span data-stu-id="003e1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="003e1-108">Щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="003e1-108">Click **Search**.</span></span>

<span data-ttu-id="003e1-109">В резултатите изберете запис за проверка.</span><span class="sxs-lookup"><span data-stu-id="003e1-109">In the results, select an audit record.</span></span> <span data-ttu-id="003e1-110">В изплаващо за подробни данни щракнете върху **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="003e1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="003e1-111">В полето **параметри** се показва информация за настройките на правилото за папка "Входящи".</span><span class="sxs-lookup"><span data-stu-id="003e1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="003e1-112">За повече информация вижте [определяне дали потребителят е създал правило за папка "Входящи"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="003e1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
