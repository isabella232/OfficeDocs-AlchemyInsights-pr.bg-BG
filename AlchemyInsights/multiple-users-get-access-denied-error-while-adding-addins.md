---
title: Няколко потребители получават грешка отказан достъп при добавяне на добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 5e5f881ad72d2a0f76c8659d6b1044bf6a18464fa8d65c079e44eb1a2afd4431
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065381"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Няколко потребители получават грешка отказан достъп при добавяне на добавки в Outlook

Можете да зададете кои администратори във вашата организация имат разрешения за инсталиране и управление на добавки за Outlook. Можете също да зададете кои потребители във вашата организация да имат разрешение да инсталират и управляват добавки за тяхна собствена употреба.

За подробности вижте [Задаване на администраторите и потребителите, които могат](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)да инсталират и управляват добавки за Outlook .

За да проверите дали сте дали успешно разрешения за даден потребител, заместете с името на ролята за проверка и изпълнете следната команда <Role Name> в Exchange Online PowerShell:

Get-ManagementRoleAssignment -Role " <Role Name> " " -GetEffectiveUsers

Този пример ви показва как да проверите на кого сте дали разрешения за инсталиране на добавки от Office store за организацията.

PowerShell

-Role "Приложения за пазара на Org" - GetEffectiveUsers

В резултатите Get-ManagementRoleAssignment прегледайте записите в колоната Ефективни потребители.

За подробна информация за синтаксиса и параметрите вижте [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 