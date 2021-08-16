---
title: Няколко потребители не виждат добавки в Outlook
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
ms.openlocfilehash: 850df2cb349f9a751def3d59fb665670e70e493daba56a88821afcef9c48ffa8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011793"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Няколко потребители не виждат добавки в Outlook

Ако тествате Outlook добавки и няма да се показват, като първа стъпка за отстраняване на неизправности, използвайте **кратката команда Get-OrganizationConfig** PowerShell, за да заявете _параметъра AppsForOfficeEnabled._ Ако заявката връща стойност False **,** задайте този параметър **на True** с помощта на **кратката команда Set-OrganizationConfig,** така че добавките да се показват по очаквания начин.

Не препоръчваме параметърът _AppsForOfficeEnabled_ да е зададен на **False**. Стойността на **False** замества всички горни настройки за административни и потребителски роли и предотвратява активирането на нови приложения от всеки потребител в организацията.

За повече информация вижте [Задаване на администраторите и потребителите,](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)които могат да инсталират и управляват добавки за Outlook .