---
title: Много потребители не виждат добавки в Outlook
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
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729860"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Много потребители не виждат добавки в Outlook

Ако тествате добавки на Outlook и нито едно не се показва, като първа стъпка за отстраняване на неизправности, използвайте кратката команда **get-OrganizationConfig** PowerShell, за да заявите параметъра _AppsForOfficeEnabled_ . Ако заявката връща стойност **FALSE**, настройте този параметър на **TRUE** с помощта на кратката команда **Set-OrganizationConfig** , така че добавките да се показват по очаквания начин.

Не препоръчваме параметърът _AppsForOfficeEnabled_ е зададен на **FALSE**. Стойността на **FALSE** отменя всички настройки по-горе за администриране и потребители и позволява на всички нови приложения да бъдат активирани от всеки потребител в организацията.

За повече информация вижте [Задаване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).