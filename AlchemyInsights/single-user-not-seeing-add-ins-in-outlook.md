---
title: Един потребител не вижда добавки в Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197735"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Един потребител не вижда добавки в Outlook

Потребителят може да е част от роля, която няма правилния параметър AppsForOfficeEnabled. Изпълнете тази команда, за да разберете дали правилната роля е свързана с потребителя:

User@domain.com за управление на $false | Формат-таблица -автоматична роля,Ролевиези име,Ролевиезитип

За повече информация вижте [Указване на администраторите и потребителите, които могат да инсталират и управляват добавки за Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
