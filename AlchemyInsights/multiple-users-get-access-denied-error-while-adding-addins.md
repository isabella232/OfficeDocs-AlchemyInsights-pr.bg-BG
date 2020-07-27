---
title: Много потребители получават грешка отказан достъп, докато добавят добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/24/2020
ms.locfileid: "45423361"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Много потребители получават грешка отказан достъп, докато добавят добавки в Outlook

Можете да укажете кои администратори във вашата организация да имат разрешения за инсталиране и управление на добавки за Outlook. Можете също да укажете кои потребители във вашата организация имат разрешение да инсталират и управляват добавки за тяхна собствена употреба.

За подробности вижте [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

За да проверите дали сте присвоили разрешения за потребител, заменя <Role Name> с името на ролята за проверка и изпълнете следната команда в Exchange Online PowerShell:

<Role Name>1000000000000000000000000000000000000000000000000000000000000

Този пример ви показва как да проверите на кого сте присвоили разрешения за инсталиране на добавки от Office хранилището за организацията.

Powershell

-Роля "Орг пазара приложения" -GetЕfectiveUsers

В резултатите Get-ManagementRoleПодписване, прегледайте записите в колоната "Ефективни потребители".

За подробна информация за синтаксиса и параметрите вижте [Получаване на управлениеRoleПодписване](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 