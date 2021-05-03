---
title: Отстраняване на неизправности в заданието за импортиране на услугата за импортиране е блокирано
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/27/2021
ms.locfileid: "52124811"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="98da5-102">Отстраняване на неизправности в заданието за импортиране на услугата за импортиране е блокирано</span><span class="sxs-lookup"><span data-stu-id="98da5-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="98da5-103">Ако имате проблеми със заданията за импортиране на услуги, блокирани или неуспешен, прегледайте и опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="98da5-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="98da5-104">Прегледайте размера на PST файла.</span><span class="sxs-lookup"><span data-stu-id="98da5-104">Review the size of of the PST file.</span></span> <span data-ttu-id="98da5-105">Максималният препоръчителен размер на PST файл за импортиране е 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="98da5-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="98da5-106">Ако подозирате, че пропуснати елементи поради повреда, изпълнете Scanpst.exe да диагностицирате и коригирате грешки в PST файлове.</span><span class="sxs-lookup"><span data-stu-id="98da5-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="98da5-107">Ако видите грешка "MapiExceptionShutoffQuotaExceeded" по време на импортиране, уверете се, че целевата пощенска кутия има достатъчен капацитет за импортиране на желаните PST файлове.</span><span class="sxs-lookup"><span data-stu-id="98da5-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="98da5-108">За повече информация относно отстраняването на проблеми с заданието за импортиране на PST вижте [Отстраняване на проблеми със задачи за импортиране на PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="98da5-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="98da5-109">За информация как да коригирате проблеми при импортиране на PSTs в Outlook вижте Коригиране на проблеми при [импортиране на Outlook .pst файл (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="98da5-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>