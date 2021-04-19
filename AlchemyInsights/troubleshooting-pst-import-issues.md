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
# <a name="troubleshooting-pst-import-issues"></a>Отстраняване на проблеми при импортиране на PST файлове

- Ако импортирате в самия клиент на Outlook, вижте [Коригиране на проблеми при импортирането на. pst файл в Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ако използвате услуга за импортиране и тя престане да се изпълнява, имайте предвид, че всеки PST файл, който качвате в местоположението за съхранение на Azure, не трябва да е по-голям от 20 ГБ. PST файлове, по-големи от 20 ГБ, може да влияят на изпълнението на процеса на импортиране на PST файлове.

- Ако искате да проверите състоянието на дадена задача за импортиране, можете да използвате кратката команда [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- За подробна информация за услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
