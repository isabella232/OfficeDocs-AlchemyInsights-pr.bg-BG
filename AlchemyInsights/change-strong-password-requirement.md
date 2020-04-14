---
title: Промяна на изискването за сигурна парола
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286238"
---
# <a name="change-strong-password-requirement"></a>Промяна на изискването за сигурна парола

Microsoft изисква надеждни пароли по подразбиране. 

С помощта на PowerShell можете да забраните силни пароли за определени потребители с тази команда:<br>
*Задаване на msolUser -Потребителскоиме–силнапаролазадължителна <UserPrincipalName> $false*

- [Повече информация за правилата за пароли](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Как да се свържете с Office 365 с PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Повече информация за командите на PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [Задаване на парола на отделен потребител да не изтече](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
