---
title: Липсващи имейли под карантина
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673703"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="ee5a5-102">Липсващи имейли в карантинни "</span><span class="sxs-lookup"><span data-stu-id="ee5a5-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="ee5a5-103">Администраторите могат да [преглеждат, отделят или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="ee5a5-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="ee5a5-104">За да отворите центъра за съответствие на защитата &, отидете на [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="ee5a5-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="ee5a5-105">За да отворите страницата карантинни директно, отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="ee5a5-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="ee5a5-106">Можете да търсите със следните стойности:</span><span class="sxs-lookup"><span data-stu-id="ee5a5-106">You can search by the following values:</span></span>  

- <span data-ttu-id="ee5a5-107">**ИД на съобщението**: глобален Еднозначен идентификатор на съобщението.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="ee5a5-108">Ако изберете съобщение в списъка, в екрана за **подробни данни** на изплаващо, който се появява, се показва СТОЙНОСТТА за **ИД на съобщението** .</span><span class="sxs-lookup"><span data-stu-id="ee5a5-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="ee5a5-109">Администраторите могат да използват [проследяването](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) на съобщенията, за да намират съобщения и СЪОТВЕТНИТЕ им ИД на съобщения.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="ee5a5-110">**Имейл адрес на подателя**: имейл адресът на един подател.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="ee5a5-111">**Имейл адрес на получателя**: имейл адресът на един получател.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="ee5a5-112">**Subject**: използвайте цялата тема на съобщението.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="ee5a5-113">Търсенето не различава малки и главни букви.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="ee5a5-114">След като въведете критериите за търсене, щракнете върху обновяване ![ на бутона Обнови, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** за да филтрирате резултатите.  </span><span class="sxs-lookup"><span data-stu-id="ee5a5-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="ee5a5-115">Кратките команди, които използвате, за да преглеждате и управлявате съобщения и файлове в карантинни депа, са:</span><span class="sxs-lookup"><span data-stu-id="ee5a5-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="ee5a5-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ee5a5-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="ee5a5-117">Експортиране – QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ee5a5-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="ee5a5-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ee5a5-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="ee5a5-119">[Визуализация – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Имайте предвид, че тази кратка команда е само за съобщения, но не и за зловреден софтуер от ATP за SharePoint Online, OneDrive за бизнеса или Teams.</span><span class="sxs-lookup"><span data-stu-id="ee5a5-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="ee5a5-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="ee5a5-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)