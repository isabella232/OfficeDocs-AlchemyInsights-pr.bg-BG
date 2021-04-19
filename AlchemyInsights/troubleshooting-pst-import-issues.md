---
title: Отстраняване на проблеми при импортиране на PST файлове
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 07609b39149c003b029f3ea5669f4044af43c25d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826152"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="14777-102">Отстраняване на проблеми при импортиране на PST файлове</span><span class="sxs-lookup"><span data-stu-id="14777-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="14777-103">Ако импортирате в самия клиент на Outlook, вижте [Коригиране на проблеми при импортирането на. pst файл в Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="14777-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="14777-104">Ако използвате услуга за импортиране и тя престане да се изпълнява, имайте предвид, че всеки PST файл, който качвате в местоположението за съхранение на Azure, не трябва да е по-голям от 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="14777-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="14777-105">PST файлове, по-големи от 20 ГБ, може да влияят на изпълнението на процеса на импортиране на PST файлове.</span><span class="sxs-lookup"><span data-stu-id="14777-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="14777-106">Ако искате да проверите състоянието на дадена задача за импортиране, можете да използвате кратката команда [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="14777-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="14777-107">За подробна информация за услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="14777-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
