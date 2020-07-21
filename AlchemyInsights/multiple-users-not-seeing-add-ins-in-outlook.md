---
title: Много потребители, които не виждат добавки в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197737"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Много потребители, които не виждат добавки в Outlook

Ако тествате Outlook добавки и никой не се появи, като първата стъпка за отстраняване на неизправности, използвайте кратката команда **Get-OrganizationConfig** PowerShell да _заявката за параметъра AppsForOfficeEnabled._ Ако заявката връща стойност на **false**, задайте този параметър **true** чрез кратката команда **Set-OrganizationConfig,** така добавки се появяват според очакванията.

Не препоръчваме параметърът _AppsForOfficeEnabled_ да е зададен **на False.** Стойността на **False** отменя всички горепосочени административни и потребителски настройки за роли и предотвратява активирането на всички нови приложения от всеки потребител в организацията.

За повече информация вж. [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).