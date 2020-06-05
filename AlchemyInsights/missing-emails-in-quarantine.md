---
title: Липсващи имейли в карантина
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568920"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="53573-102">Липсващи имейли в карантина"</span><span class="sxs-lookup"><span data-stu-id="53573-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="53573-103">Администраторите могат да [преглеждат, освобождават или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="53573-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="53573-104">За да отворите Центъра за съответствие на & за защита, отидете на [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="53573-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="53573-105">За да отворите директно страницата "Карантина", отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="53573-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="53573-106">Можете да търсите по следните стойности:</span><span class="sxs-lookup"><span data-stu-id="53573-106">You can search by the following values:</span></span>  

- <span data-ttu-id="53573-107">**ИД**на съобщение : Глобално еднозначен идентификатор на съобщението.</span><span class="sxs-lookup"><span data-stu-id="53573-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="53573-108">Ако изберете съобщение в списъка, стойността на **ИД** на съобщение се появява в екрана за допълнителни **подробности,** който се появява.</span><span class="sxs-lookup"><span data-stu-id="53573-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="53573-109">Администраторите могат да използват [съобщение за проследяване](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) за намиране на съобщения и съответните им стойности за ИД на съобщение.</span><span class="sxs-lookup"><span data-stu-id="53573-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="53573-110">**Имейл адрес на подателя:** Имейл адрес на един единствен подател.</span><span class="sxs-lookup"><span data-stu-id="53573-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="53573-111">**Имейл адрес на получателя:** Имейл адрес на един получател.</span><span class="sxs-lookup"><span data-stu-id="53573-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="53573-112">**Относно:** Използвайте целия предмет на съобщението.</span><span class="sxs-lookup"><span data-stu-id="53573-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="53573-113">Търсенето не е от значение за малките и главните букви.</span><span class="sxs-lookup"><span data-stu-id="53573-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="53573-114">След като въведете критериите за търсене, щракнете върху ![ Бутона ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обновяване,** за да филтрирате резултатите.  </span><span class="sxs-lookup"><span data-stu-id="53573-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="53573-115">Кратките команди, които използвате за преглед и управлява съобщения и файлове в карантина са:</span><span class="sxs-lookup"><span data-stu-id="53573-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="53573-116">Изтриване на карантинаСъсижен</span><span class="sxs-lookup"><span data-stu-id="53573-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="53573-117">Експортиране-карантинаСъсище</span><span class="sxs-lookup"><span data-stu-id="53573-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="53573-118">Получаване на карантина:</span><span class="sxs-lookup"><span data-stu-id="53573-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="53573-119">[Визуализация-карантинаСъс кутия:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Имайте предвид, че тази команда е само за съобщения, а не зловреден софтуер файлове от ATP за SharePoint Online, OneDrive за бизнес или екипи.</span><span class="sxs-lookup"><span data-stu-id="53573-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="53573-120">Карантина за освобождаване</span><span class="sxs-lookup"><span data-stu-id="53573-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)