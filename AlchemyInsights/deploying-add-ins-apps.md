---
title: Разполагане на добавки за Приложения на Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233502"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Разполагане на добавки за Приложения на Microsoft 365

Централизирано разполагане е препоръчителният начин за разполагане Office добавки за потребители и групи във вашата организация. За да разположите добавки, изпълнете стъпките по-долу:

**Забележка:** За да инсталирате добавки за Office като отделен потребител, вижте [Преглед, управление](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)и инсталиране на добавки в Office програми . Също така се уверете, че е разрешено индивидуално Office на добавки в магазина. За подробности вижте Предотвратяване на изтегляния на добавки, като изключите Office store за всички клиенти [(с изключение Outlook)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook).

1. Уверете се, че вашата среда отговаря на изискванията за разполагане на добавки с помощта на централизирано разполагане. За подробности вижте [Изисквания](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Отидете на **Настройки** Приложения Получаване на приложения  >    >   в центъра за Microsoft 365 за администриране, за да разположите добавки. 

Бележки: 

- Интегрираните приложения изискват администраторът да има разрешения за глобален администратор или Exchange администратор.

- Когато разполагате добавки за няколко потребители, ви препоръчваме да извършвате задачи с помощта на групи, а не на отделни потребители. За подробности вижте [Съображения при присвояване на добавка към потребители и групи](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).

- Централизирано разполагане не поддържа потребители в вложени групи или групи, които имат родителски групи. За подробности вижте [Задачи на потребител и група](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- Уверете се, че услугата за управление на приложения на Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') е разрешена за влизане от потребителите. За подробности вижте Конфигуриране [на свойствата на приложението](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- Ако имате проблеми с разполагането на добавки с помощта на интегрирани приложения, опитайте да разположите [с помощта на добавки](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).

За повече информация вижте:

[Разполагане на добавки в центъра за администриране](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Управление на добавки в центъра за администриране](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Използване на кратки команди на PowerShell за централизирано разполагане за управление на добавки](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Публикуване Office добавки с помощта на централизирано разполагане чрез центъра Microsoft 365 администриране](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Отстраняване на неизправности: Потребител не вижда добавки](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Отстраняване на грешки на потребители Office добавки](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)