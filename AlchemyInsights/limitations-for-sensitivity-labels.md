---
title: Ограничения за етикетите за чувствителност за Office файлове в SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e197c43712c0ead9508a1cfdf48b51d01d2ae957649f73703f9c33733e332bf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813149"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>Ограничения за етикетите за чувствителност за Office файлове в SharePoint и OneDrive

Когато разрешавате етикети за чувствителност за Office файлове в SharePoint и OneDrive, имайте предвид изискванията и ограниченията, които включват:

- SharePoint и OneDrive не могат да обработват някои файлове, етикетирани и шифровани от настолни приложения на Office, когато файловете съдържат данни на PowerQuery, данни, съхранявани от добавки по избор или XML части по избор.
- SharePoint и OneDrive не прилагат автоматично етикети за чувствителност към съществуващи файлове, които вече сте шифровали с помощта на етикети за защита на информацията в Azure (AIP). За да приложите етикети за чувствителност към шифровани файлове: 
    - Уверете се, че AIP етикетите са мигрирани и публикувани в центъра за Microsoft 365 съответствие.
    - Изтеглете етикетираните файлове и след това ги качете в първоначалното им SharePoint или OneDrive местоположение.
- За шифровани документи печатът не се поддържа.

За допълнителни подробности относно ограниченията вижте Разрешаване на етикети за чувствителност [за Office файлове в SharePoint и OneDrive.](/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)
