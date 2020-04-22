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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706550"
---
# <a name="change-strong-password-requirement"></a>Промяна на изискването за сигурна парола

Microsoft изисква надеждни пароли по подразбиране. 

С помощта на PowerShell можете да забраните силни пароли за определени потребители с тази команда:<br>
*Задаване на msolUser -Потребителскоиме–силнапаролазадължителна <UserPrincipalName> $false*

- [Повече информация за правилата за пароли](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Как да се свържете с Microsoft 365 с PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Повече информация за командите на PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
