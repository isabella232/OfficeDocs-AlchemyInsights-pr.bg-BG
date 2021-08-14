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
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972408"
---
# <a name="troubleshooting-pst-import-issues"></a>Отстраняване на проблеми при импортиране на PST файлове

- Ако импортирате в самия клиент Outlook, вижте Коригиране на проблеми при [импортиране на Outlook .pst файл](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Ако използвате услугата за импортиране и тя е блокирана, обърнете внимание, че всеки PST файл, който качвате в местоположението за съхранение в Azure, не трябва да е по-голям от 20 ГБ. PST файловете, по-големи от 20 ГБ, може да влияят върху производителността на процеса на импортиране чрез PST. За повече информация относно отстраняването на неизправности при задания за блокиране вижте [Проблеми, които засягат задачи за импортиране на PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

- Ако искате да проверите състоянието на конкретно задание за импортиране, използвайте [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- За пълни подробности относно услугата за импортиране вижте [Общ преглед на импортирането на PST файловете на вашата организация.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
