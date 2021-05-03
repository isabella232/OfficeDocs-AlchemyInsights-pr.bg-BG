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
# <a name="troubleshooting-import-service-job-stuck"></a>Отстраняване на неизправности в заданието за импортиране на услугата за импортиране е блокирано

Ако имате проблеми със заданията за импортиране на услуги, блокирани или неуспешен, прегледайте и опитайте следното:

- Прегледайте размера на PST файла. Максималният препоръчителен размер на PST файл за импортиране е 20 ГБ.

- Ако подозирате, че пропуснати елементи поради повреда, изпълнете Scanpst.exe да диагностицирате и коригирате грешки в PST файлове.

- Ако видите грешка "MapiExceptionShutoffQuotaExceeded" по време на импортиране, уверете се, че целевата пощенска кутия има достатъчен капацитет за импортиране на желаните PST файлове.

За повече информация относно отстраняването на проблеми с заданието за импортиране на PST вижте [Отстраняване на проблеми със задачи за импортиране на PST](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).

За информация как да коригирате проблеми при импортиране на PSTs в Outlook вижте Коригиране на проблеми при [импортиране на Outlook .pst файл (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).