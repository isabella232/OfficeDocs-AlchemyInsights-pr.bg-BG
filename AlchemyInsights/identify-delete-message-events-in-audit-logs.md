---
title: Идентифициране на събития при изтриване на съобщения в регистрационни файлове за проверка
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696502"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="9c873-102">Регистрационни файлове за проверка на изтрити имейл съобщения</span><span class="sxs-lookup"><span data-stu-id="9c873-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="9c873-103">Започвайки от януари 2019, Microsoft се включва в регистрирането на проверката на пощенска кутия по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="9c873-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="9c873-104">В противен случай, за да прегледате съобщения за изтриване на събития за определен потребител, трябва ръчно да разрешите действията за изтриване за проверка.</span><span class="sxs-lookup"><span data-stu-id="9c873-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="9c873-105">Ако регистрирането на проверката на пощенска кутия вече е разрешено за вашата организация или за определен потребител, следвайте стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="9c873-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="9c873-106">Влезте в центъра за [съответствие на & на Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="9c873-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9c873-107">Щракнете върху **търсене и проучване** и изберете **търсене в регистрационния файл за проверка**.</span><span class="sxs-lookup"><span data-stu-id="9c873-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9c873-108">Изберете диапазона от дати в полетата " **Начална дата** " и " **крайна дата** ".</span><span class="sxs-lookup"><span data-stu-id="9c873-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9c873-109">Укажете потребителско име за потребителя, който искате да изследвате (потребителят, който е изтрил елементите).</span><span class="sxs-lookup"><span data-stu-id="9c873-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="9c873-110">В полето **дейности** изберете **изтрити съобщения от папката "Изтрити"** и **преместени съобщения в папката "Изтрити елементи**".</span><span class="sxs-lookup"><span data-stu-id="9c873-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="9c873-111">Щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="9c873-111">Click **Search**.</span></span>

<span data-ttu-id="9c873-112">В резултатите изберете запис за проверка.</span><span class="sxs-lookup"><span data-stu-id="9c873-112">In the results, select an audit record.</span></span> <span data-ttu-id="9c873-113">В изплаващо за подробни данни щракнете върху **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="9c873-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9c873-114">Допълнителна информация относно изтрит елемент (например редът за тема и местоположението на елемента, когато е бил изтрит) се показва в полето **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="9c873-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="9c873-115">Свойството **ClientInfoString** ще покаже, че изтриването е възникнало в Outlook, Outlook в уеб (наричан преди това Outlook Web App) или друго устройство.</span><span class="sxs-lookup"><span data-stu-id="9c873-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="9c873-116">За повече информация вижте [определяне кой е настроил препращане на имейл за пощенска кутия](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="9c873-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="9c873-117">**Забележка**: не можете да извличате изтрити елементи с помощта на функцията за регистрационен файл за проверка.</span><span class="sxs-lookup"><span data-stu-id="9c873-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="9c873-118">За да възстановите изтритите съобщения в Outlook в уеб, вижте [възстановяване на изтрити елементи в Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="9c873-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
