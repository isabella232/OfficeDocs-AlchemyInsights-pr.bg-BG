---
title: Проблеми с лицензирането на Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148181"
---
# <a name="yammer-licensing-issues"></a>Проблеми с лицензирането на Yammer

Всички потребители трябва да имат лиценз за използване на yammer Enterprise услуга, но по подразбиране Yammer не изисква потребителите да имат лиценз за достъп до услугата. Когато администратор променя настройката да блокирате потребителите на Microsoft 365 без Yammer лицензи, потребителите не присвоени Yammer Enterprise лиценз не достъп до услугата Yammer. За повече информация вижте [управление на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Когато лицензи се премахват от потребителите, Yammer плочка вече не се показва и други услуги да използвате лиценз за премахване на функции. В други случаи характеристиките могат да се появят, но изискват да се извършва възлагането на лиценз.  

**Лицензът не се актуализира за потребителя**  

Понякога потребител е присвоен лиценз, но все още не може да достъп до Yammer. Закъсненията са по-склонни да се случат, когато се извършва масово възлагане на лицензи. Yammer потребители може да не се актуализира в същия ред като лицензи се променят в Azure AD защото системата работи асинхронно. Изчакайте до 24 часа, преди да отворите случай с поддръжка, за да съобщите за проблеми със синхронизирането на лицензи.  

**Разпределяне на насипни лицензии**  

Лицензи могат да бъдат присвоени чрез център за администриране или PowerShell скриптове. За повече информация вижте [Присвояване на лицензи на потребители](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и [Присвояване на лицензи към потребителски акаунти с Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Поддръжката на Microsoft не предоставя помощ при създаване на скриптове, но документация за Присвояване на Yammer лиценз е налична. За повече информация вижте [Управление на Yammer лицензи с помощта на Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).