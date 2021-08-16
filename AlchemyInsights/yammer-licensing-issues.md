---
title: Yammer проблеми с лицензирането
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989718"
---
# <a name="yammer-licensing-issues"></a>Yammer проблеми с лицензирането

Всички потребители трябва да имат лиценз за използване Yammer Enterprise услугата, но по подразбиране Yammer не изисква потребителите да имат лиценз за достъп до услугата. Когато администратор промени настройката, за да блокира Microsoft 365 потребители без лицензи Yammer, потребителите, на които не е присвоен лиценз за Yammer Enterprise, няма да имат достъп до Yammer услугата. За повече информация вижте Управление [на Yammer потребителски лицензи в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Когато лицензите се премахват от потребители, плочката Yammer вече не се показва, а други услуги могат да използват премахването на лицензи, за да скрият функциите. В други случаи функциите все още могат да се показват, но изискват назначаване на лиценз за работа.  

**Лицензът не се актуализира за потребителя**  

Понякога на даден потребител се дава лиценз, но все още не може да получи достъп Yammer. Има по-голяма вероятност да възникнат закъснения, когато се в ход се присвояване на масов лиценз. Yammer може да не се актуализират в същия ред като лицензите в Azure AD, тъй като системата се изпълнява асинхронно. Изчакайте до 24 часа, преди да отворите случай на поддръжка, за да съобщите за проблеми със синхронизирането на лицензи.  

**Групово присвояване на лицензи**  

Лицензите могат да бъдат присвоени чрез центъра за администриране или скриптовете на PowerShell. За повече информация вижте [Дайте лицензи на потребители и](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [Дайте лицензи на потребителски акаунти с Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Поддръжката на Microsoft не предоставя помощ при създаването на скриптове, но е налична документация Yammer на лицензи. За повече информация вижте Управление [на Yammer лицензи с помощта на Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).