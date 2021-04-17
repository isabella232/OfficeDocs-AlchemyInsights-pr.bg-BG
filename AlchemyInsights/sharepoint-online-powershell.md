---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830571"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Работа с PowerShell или скриптове в Sharepoint Online? Посетете връзките по-долу за повече информация.
- [Първи стъпки в обвивката за управление на SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Свързване към SPO PowerShell с многофакторно удостоверяване (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [Моделите и практиките на SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) съдържат библиотека с команди на PowerShell, която ви позволява да извършвате сложни действия за управление към SPO.

> [!NOTE]
> - Ако имате проблеми със свързването с обвивката за управление на SPO, уверете се, че сте актуализирали до [най-новата](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) версия и се опитайте да импортирате отново модула с *помощта на "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Ако се опитвате да изпълните скриптове за обектен модел от страната на клиента, ще трябва да имате инсталиран SDK за клиентски компоненти на [SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) на вашия локален компютър.
> - Ако имате проблеми с изпълнението на скриптове от PowerShell, може да помислите да изпълните PowerShell като администратор и да промените правилата [за изпълнение.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)