---
title: Потребителската картина все още се показва в Microsoft Teams организационна диаграма
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422184"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Потребителската картина все още се показва в Microsoft Teams организационна диаграма

Ако един или повече лица във вашата организация са дезактивирани или премахнати и снимката на профила им все още се показва в организационната диаграма, е възможно настройката **ShowInAddressLists** да е зададена на False: 

1. Отидете на Център за администриране на Microsoft 365 > [активни потребители и](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) изберете потребителя със снимката, която все още се показва. 
1. Изберете раздела **Поща** и се уверете, че **Показване в глобалния адресен списък е** зададено на **Не**.

Ако **настройката ShowInAddressLists** на **Не** не работи, проверете следното: 

- Потребителят може да бъде показан от списъка на получателите в Exchange. За повече информация вижте Управление [на адресни списъци в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Потребителят може да бъде показан от адресния списък в Azure Active Directory. За повече информация вижте [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 