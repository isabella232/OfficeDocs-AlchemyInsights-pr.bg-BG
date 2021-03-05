---
title: Четене на регистрационни файлове за проверка за изтрити събития
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481015"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="1d05c-102">Четене на регистрационни файлове за проверка за изтрити събития</span><span class="sxs-lookup"><span data-stu-id="1d05c-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="1d05c-103">Ето как да направите това:</span><span class="sxs-lookup"><span data-stu-id="1d05c-103">Here's how to do this:</span></span>

1. <span data-ttu-id="1d05c-104">Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="1d05c-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="1d05c-105">Изберете **търсене** в  >  [**регистрационния файл за проверка**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="1d05c-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="1d05c-106">Ако видите съобщение, което ви трябва, за да включите функцията, продължете напред и го включете сега.</span><span class="sxs-lookup"><span data-stu-id="1d05c-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="1d05c-107">Ако функцията не е включена, резултатите от търсенето няма да могат да изтеглят данни от предишни дати.</span><span class="sxs-lookup"><span data-stu-id="1d05c-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="1d05c-108">Изберете **дейности** и след това намерете **дейности за пощенска кутия на Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1d05c-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="1d05c-109">Изберете **изтритите съобщения от** папката "Изтрити" и **преместените съобщения в опциите за папката "Изтрити елементи** ".</span><span class="sxs-lookup"><span data-stu-id="1d05c-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="1d05c-110">Когато сте готови, щракнете извън екрана, за да намалите екрана **дейности** .</span><span class="sxs-lookup"><span data-stu-id="1d05c-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="1d05c-111">Задайте диапазона от дати и след това в полето **потребители** изберете потребителското име за потребителя, който искате да изследвате.</span><span class="sxs-lookup"><span data-stu-id="1d05c-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="1d05c-112">Можете да изберете повече от един потребител едновременно.</span><span class="sxs-lookup"><span data-stu-id="1d05c-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="1d05c-113">Изберете **търсене**.</span><span class="sxs-lookup"><span data-stu-id="1d05c-113">Select **Search**.</span></span> <span data-ttu-id="1d05c-114">Дейността се показва под **резултати**.</span><span class="sxs-lookup"><span data-stu-id="1d05c-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="1d05c-115">За да прегледате подробностите, изберете дейност и след това изберете **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="1d05c-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="1d05c-116">Допълнителна информация относно изтрит елемент, като например реда за тема и местоположението на елемента, когато е бил изтрит, се показва в полето **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="1d05c-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="1d05c-117">Не можете да възстановите изтрити елементи с помощта на функцията за регистриране на проверката.</span><span class="sxs-lookup"><span data-stu-id="1d05c-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="1d05c-118">За възстановяване на изтрити елементи вижте [възстановяване на изтрити елементи или имейл в Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="1d05c-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="1d05c-119">За да научите повече, вижте [търсене в регистрационния файл за проверка на Office 365 за отстраняване на често срещани сценарии](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="1d05c-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
