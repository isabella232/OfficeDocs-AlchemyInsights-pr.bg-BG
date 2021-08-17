---
title: Един потребител не вижда добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050647"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Един потребител не вижда добавки в Outlook

Потребителят може да е част от роля, която няма правилния параметър AppsForOfficeEnabled. Изпълнете тази кратка команда, за да разберете дали правилната роля е свързана с потребителя:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

За повече информация вижте [Задаване на администраторите и потребителите,](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)които могат да инсталират и управляват добавки за Outlook.
