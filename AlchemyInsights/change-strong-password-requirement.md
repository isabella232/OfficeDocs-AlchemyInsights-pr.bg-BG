---
title: Промяна на изискването за сигурна парола
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8a82c002bd64a33556b632545e98355e860848d845e122bfea06fbc5ee5dcb90
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070673"
---
# <a name="change-strong-password-requirement"></a>Промяна на изискването за сигурна парола

Microsoft изисква сигурни пароли по подразбиране.

С помощта на PowerShell можете да забраните сигурни пароли за определени потребители с тези команди:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

За да забраните сигурни пароли за всички потребители, използвайте:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Повече информация за правилата за пароли](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Как да се свържете с Microsoft 365 с PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Повече информация за командите на PowerShell за MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
