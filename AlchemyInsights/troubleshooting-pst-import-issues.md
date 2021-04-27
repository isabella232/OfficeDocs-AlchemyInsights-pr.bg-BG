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
# <a name="troubleshooting-pst-import-issues"></a>Отстраняване на проблеми при импортиране на PST файлове

- Ако импортирате в самия клиент на Outlook, вижте Коригиране на [проблеми при импортиране на .pst файл на Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ако използвате услугата за импортиране и тя е блокирана, обърнете внимание, че всеки PST файл, който качвате в местоположението за съхранение в Azure, не трябва да е по-голям от 20 ГБ. PST файловете, по-големи от 20 ГБ, може да влияят върху производителността на процеса на импортиране чрез PST. За повече информация относно отстраняването на неизправности при задания за блокиране вижте [Проблеми, които засягат задачи за импортиране на PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Ако искате да проверите състоянието на конкретно задание за импортиране, използвайте [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- За пълни подробности относно услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
