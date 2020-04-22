---
title: Идентифициране на изтриване на събития та в регистрационните файлове за проверка
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
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716485"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="bc87c-102">Регистрационни файлове за проверка за изтрити имейл съобщения</span><span class="sxs-lookup"><span data-stu-id="bc87c-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="bc87c-103">Започва йки през януари 2019 г., Microsoft включва проверка на пощенска кутия регистриране по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="bc87c-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="bc87c-104">В противен случай, за да прегледате изтриването на събития та съобщения за конкретен потребител, трябва ръчно да разрешите изтриване то действия та проверка.</span><span class="sxs-lookup"><span data-stu-id="bc87c-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="bc87c-105">Ако регистрирането на проверка на пощенска кутия вече е разрешено за вашата организация или за конкретен потребител, изпълнете стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="bc87c-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="bc87c-106">Влезте в центъра за съответствие на & за защита на [Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="bc87c-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="bc87c-107">Щракнете върху **Търсене и разследване** и изберете Търсене на **регистрационен файл за проверка**.</span><span class="sxs-lookup"><span data-stu-id="bc87c-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="bc87c-108">Изберете периода от време в полетата **Начална дата** и **Крайна дата.**</span><span class="sxs-lookup"><span data-stu-id="bc87c-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="bc87c-109">Задайте потребителско име за потребителя, който искате да проучи (потребителят, който е изтрил елементите).</span><span class="sxs-lookup"><span data-stu-id="bc87c-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="bc87c-110">В полето **Дейности** изберете **Изтрити съобщения от папката "Изтрити"** и **преместени съобщения в папката "Изтрити елементи".**</span><span class="sxs-lookup"><span data-stu-id="bc87c-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="bc87c-111">Щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="bc87c-111">Click **Search**.</span></span>

<span data-ttu-id="bc87c-112">В резултатите изберете запис за проверка.</span><span class="sxs-lookup"><span data-stu-id="bc87c-112">In the results, select an audit record.</span></span> <span data-ttu-id="bc87c-113">В допълнителното меню за подробни данни щракнете върху **Още информация**.</span><span class="sxs-lookup"><span data-stu-id="bc87c-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="bc87c-114">Допълнителна информация за изтрития елемент (например темата и местоположението на елемента, когато е изтрит) се показва в полето **"Засегнати елементи".**</span><span class="sxs-lookup"><span data-stu-id="bc87c-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="bc87c-115">Свойството **ClientInfoString** ще покаже дали изтриването е възникнало в Outlook, Outlook в уеб (по-рано известен като Outlook Web App) или всяко друго устройство.</span><span class="sxs-lookup"><span data-stu-id="bc87c-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="bc87c-116">За повече информация вижте [Определяне кой да настроите имейл препращане за пощенска кутия](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="bc87c-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="bc87c-117">**Забележка:** Не можете да извлечете изтритите елементи с помощта на функцията за проверка на регистрационния файл.</span><span class="sxs-lookup"><span data-stu-id="bc87c-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="bc87c-118">За да извлечете изтрити съобщения в Outlook в мрежата, вижте [Възстановяване на изтритите елементи в Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="bc87c-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
