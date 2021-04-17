---
title: Липсващи имейли под карантина
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831723"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="bcfb1-102">Липсващи имейли под карантина"</span><span class="sxs-lookup"><span data-stu-id="bcfb1-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="bcfb1-103">Администраторите могат [да преглеждат, пускат или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="bcfb1-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="bcfb1-104">За да отворите центъра за & за съответствие, отидете на [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="bcfb1-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="bcfb1-105">За да отворите страницата Карантина директно, отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="bcfb1-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="bcfb1-106">Можете да търсите по следните стойности:</span><span class="sxs-lookup"><span data-stu-id="bcfb1-106">You can search by the following values:</span></span>  

- <span data-ttu-id="bcfb1-107">**ИД на** съобщение: Глобално уникалният идентификатор на съобщението.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="bcfb1-108">Ако изберете съобщение в списъка, стойността на  **ИД**  на съобщението се показва в екрана с допълнителни  **данни,**  който се появява.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="bcfb1-109">Администраторите могат да използват [проследяване на съобщения,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) за да намират съобщения и съответните им стойности за ИД на съобщение.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="bcfb1-110">**Имейл адрес на подателя:** Имейл адрес на един подател.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="bcfb1-111">**Имейл адрес на** получателя: Имейл адрес на един получател.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="bcfb1-112">**Тема:** Използвайте цялата тема на съобщението.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="bcfb1-113">Търсенето не е с малки и главни букви.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="bcfb1-114">След като сте въвели критериите за търсене, щракнете върху бутона ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обнови, за** да филтрирате резултатите.  </span><span class="sxs-lookup"><span data-stu-id="bcfb1-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="bcfb1-115">Кратките команди, които използвате за преглед и управление на съобщения и файлове под карантина, са:</span><span class="sxs-lookup"><span data-stu-id="bcfb1-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="bcfb1-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bcfb1-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="bcfb1-117">Експортиране-карантинаMessage</span><span class="sxs-lookup"><span data-stu-id="bcfb1-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="bcfb1-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="bcfb1-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="bcfb1-119">[Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обърнете внимание, че тази кратка команда е само за съобщения, а не за злонамерени файлове от ATP за SharePoint Online, OneDrive за бизнеса или Teams.</span><span class="sxs-lookup"><span data-stu-id="bcfb1-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="bcfb1-120">Съобщение за карантинаMessage</span><span class="sxs-lookup"><span data-stu-id="bcfb1-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)