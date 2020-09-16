---
title: Грешка "много потребители получавате отказан достъп" при добавяне на добавки в Outlook
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724352"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Грешка "много потребители получавате отказан достъп" при добавяне на добавки в Outlook

Можете да зададете кои администратори във вашата организация да имат разрешения за инсталиране и управление на добавки за Outlook. Можете също да укажете кои потребители във вашата организация да имат разрешение за инсталиране и управление на добавки за тяхна собствена употреба.

За подробности вижте [Задаване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

За да се уверите, че сте задали успешно разрешения за потребител, заменете <Role Name> с името на ролята за проверка и изпълнете следната команда в PowerShell на Exchange Online:

Get-ManagementRoleAssignment-роля " <Role Name> "-GetEffectiveUsers

Този пример ви показва как да проверите кого сте задали разрешения за инсталиране на добавки от Office магазина за организацията.

PowerShell

-Роля "приложения за пазара на org" – GetEffectiveUsers

В резултатите Получете ManagementRoleAssignment, прегледайте записите в колоната за ефективни потребители.

За подробен синтаксис и информация за параметрите вижте [get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 