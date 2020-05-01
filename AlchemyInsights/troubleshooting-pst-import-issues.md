---
title: Отстраняване на проблеми при импортиране на PST файлове
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991087"
---
# <a name="troubleshooting-pst-import-issues"></a>Отстраняване на проблеми при импортиране на PST файлове

- Ако импортирате в самия клиент на Outlook, вижте [Коригиране на проблеми при импортирането на. pst файл в Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ако използвате услуга за импортиране и тя престане да се изпълнява, имайте предвид, че всеки PST файл, който качвате в местоположението за съхранение на Azure, не трябва да е по-голям от 20 ГБ. PST файлове, по-големи от 20 ГБ, може да влияят на изпълнението на процеса на импортиране на PST файлове.

- Ако искате да проверите състоянието на дадена задача за импортиране, можете да използвате кратката команда [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- За подробна информация за услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
