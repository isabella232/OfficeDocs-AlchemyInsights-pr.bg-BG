---
title: Идентифициране на събитията от изтриване на съобщения в регистрационните файлове
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508977"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="41925-102">Регистрационни файлове за проверка на изтрити имейл съобщения</span><span class="sxs-lookup"><span data-stu-id="41925-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="41925-103">Започвайки през януари 2019, Microsoft се включва пощенска кутия проверка регистриране по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="41925-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="41925-104">В противен случай, за да прегледате събитията за изтриване на съобщения за конкретен потребител, трябва ръчно да разрешите действията за изтриване за проверка.</span><span class="sxs-lookup"><span data-stu-id="41925-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="41925-105">Ако проверка на пощенска кутия регистриране вече е разрешено за вашата организация или за конкретен потребител, изпълнете стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="41925-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="41925-106">Влезте в центъра за съответствие на [microsoft 365 защита &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="41925-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="41925-107">Щракнете върху **Търсене и разследване** и изберете Търсене в регистрационния файл за **проверка**.</span><span class="sxs-lookup"><span data-stu-id="41925-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="41925-108">Изберете периода от време в полетата **Начална дата** и **Крайна дата.**</span><span class="sxs-lookup"><span data-stu-id="41925-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="41925-109">Задайте потребителско име за потребителя, който искате да проучи (потребителят, който е изтрил елементите).</span><span class="sxs-lookup"><span data-stu-id="41925-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="41925-110">В полето **Дейности** изберете **Изтрити съобщения от папката "Изтрити елементи"** и **"Преместени съобщения" в папка "Изтрити"**.</span><span class="sxs-lookup"><span data-stu-id="41925-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="41925-111">Щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="41925-111">Click **Search**.</span></span>

<span data-ttu-id="41925-112">В резултатите изберете запис за проверка.</span><span class="sxs-lookup"><span data-stu-id="41925-112">In the results, select an audit record.</span></span> <span data-ttu-id="41925-113">В допълнителните подробности щракнете върху **"Повече информация"**.</span><span class="sxs-lookup"><span data-stu-id="41925-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="41925-114">Допълнителна информация за изтрити елемент (например тема и местоположението на елемента, когато е бил изтрит) се показва в полето **Засегнати елементи** .</span><span class="sxs-lookup"><span data-stu-id="41925-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="41925-115">Свойството **ClientInfoString** ще покаже, ако изтриването е възникнало в Outlook, Outlook в мрежата (преди това като Outlook Web App) или всяко друго устройство.</span><span class="sxs-lookup"><span data-stu-id="41925-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="41925-116">За повече информация вижте [Определяне кой настройва изпращане на имейл за пощенска кутия](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="41925-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="41925-117">**Забележка:** Не можете да извлечете изтрити елементи с помощта на функцията за регистрационен файл за проверка.</span><span class="sxs-lookup"><span data-stu-id="41925-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="41925-118">За да извлечете изтрити съобщения в Outlook в мрежата, вижте [Възстановяване на изтрити елементи в Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="41925-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
