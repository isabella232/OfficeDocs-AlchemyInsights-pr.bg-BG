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
ms.openlocfilehash: 5065b9895954371e4298c98e8aadb67ba8f140fd
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059804"
---
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="7573c-102">Отстраняване на проблеми при импортиране на PST файлове</span><span class="sxs-lookup"><span data-stu-id="7573c-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="7573c-103">Ако импортирате в самия клиент на Outlook, вижте Коригиране на [проблеми при импортиране на .pst файл на Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="7573c-103">If you are importing within the Outlook client itself, see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="7573c-104">Ако използвате услугата за импортиране и тя е блокирана, обърнете внимание, че всеки PST файл, който качвате в местоположението за съхранение в Azure, не трябва да е по-голям от 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="7573c-104">If you are using Import Service and it's stuck, note that each PST file that you upload to the Azure Storage location should be no larger than 20GB.</span></span> <span data-ttu-id="7573c-105">PST файловете, по-големи от 20 ГБ, може да влияят върху производителността на процеса на импортиране чрез PST.</span><span class="sxs-lookup"><span data-stu-id="7573c-105">PST files larger than 20GB may impact the performance of the PST import process.</span></span> <span data-ttu-id="7573c-106">За повече информация относно отстраняването на неизправности при задания за блокиране вижте [Проблеми, които засягат задачи за импортиране на PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="7573c-106">For more information troubleshooting stuck jobs, see [Issues that affect PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

- <span data-ttu-id="7573c-107">Ако искате да проверите състоянието на конкретно задание за импортиране, използвайте [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="7573c-107">If you want to verify the status of a specific Import job, use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="7573c-108">За пълни подробности относно услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="7573c-108">For full details on the import service, see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
