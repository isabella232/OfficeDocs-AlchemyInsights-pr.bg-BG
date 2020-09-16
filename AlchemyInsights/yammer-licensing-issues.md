---
title: Проблеми с лицензирането в Yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657265"
---
# <a name="yammer-licensing-issues"></a>Проблеми с лицензирането в Yammer

Всички потребители трябва да имат лиценз за използване на услугата Yammer Enterprise, но по подразбиране Yammer не изисква потребителите да имат лиценз за достъп до услугата. Когато администратор промени настройката за блокиране на потребители на Microsoft 365 без лицензи на Yammer, потребителите, на които не е даден лиценз за yammer Enterprise, нямат достъп до услугата Yammer. За повече информация вижте [управление на потребителските лицензи за Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Когато лицензи се премахват от потребители, плочката Yammer вече не се показва и други услуги могат да използват премахването на лицензи, за да скриват функции. В други случаи функциите все още могат да се появяват, но изисква присвояване на лиценз за работа.  

**Лицензът не се актуализира за потребителя**  

Понякога на даден потребител е присвоен лиценз, но все още не може да получи достъп до Yammer. Забавянето е по-вероятно да възникне, когато се изпълнява задача за масово лицензиране. Потребителите на Yammer може да не се актуализират по същия начин, по който се променят лицензите в Azure AD, тъй като системата се стартира асинхронно. Изчакайте до 24 часа, преди да отворите калъф за поддръжка, за да съобщите за проблеми при синхронизиране на лицензи.  

**Присвояване на групови лицензи**  

Лицензи могат да бъдат присвоени чрез скриптове на центъра за администриране или PowerShell. За повече информация вижте даване [на лицензи на потребители](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) и даване [на лицензи на потребителски акаунти с Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Поддръжката на Microsoft не предоставя съдействие при създаването на скриптове, но документацията за даване на лиценз за Yammer е налична. За повече информация вижте [управление на лицензи за Yammer с помощта на Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).