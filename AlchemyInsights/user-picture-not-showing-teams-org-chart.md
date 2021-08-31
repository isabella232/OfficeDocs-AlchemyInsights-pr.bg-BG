---
title: Потребителската картина не се показва Microsoft Teams организационна диаграма
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792642"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Потребителската картина не се показва Microsoft Teams организационна диаграма

Ако на една или повече лица във вашата организация липсва снимката на профила в организационната диаграма, е възможно настройката **ShowInAddressLists** да е зададена на **False:**

1. Отидете на Център за администриране на Microsoft 365 > [**активни потребители**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)и изберете потребителя с липсващата снимка. 
1. Изберете раздела **Поща** и се уверете, че **Показване в глобалния адресен списък** е зададено на **Да**. 

Ако **настройката ShowInAddressLists** **на Yes** не работи, проверете следното:

- Потребителят може да е скрит от списъка с получатели в Exchange. За повече информация вижте Управление [на адресни списъци в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Потребителят може да е скрит от адресния списък в Azure Active Directory. За повече информация вижте [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
