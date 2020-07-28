---
title: Не може да се промени потребителско име
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438785"
---
# <a name="unable-to-change-username"></a>Не може да се промени потребителско име

В някои случаи UPN (UserPrincipalName) промени не се разпространяват в облака. Може да получите грешки при проверка в портала на Office 365 или да не можете да промените потребителското име или имейл адреса. За да разрешите този проблем, ръчно задайте UserPrincipalName с помощта на тази команда PowerShell .

**Пример: Преименуване на потребител**

PowerShellCopy

PS C: \> Задайте MsolUserPrincipalName - Потребителско име на потребителя "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

Тази команда преименува davidc@contoso.com на davidchew@contoso.com.

За повече информация вижте [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).