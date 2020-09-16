---
title: Изтриване на потребител, който е сирак от локален сървър
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680124"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Изтриване на потребител, който е сирак от локален сървър

За да премахнете потребител, който е сирак, изпълнете следните стъпки:

1. Синхронизиране на форс справочен указател, като следвате инструкциите в [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. За проверка на синхронизирането на справочен указател вижте [Какво представлява хибридната самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ако функциите за синхронизиране са правилни, но изтриването на обекти на Active Directory не се разпространява в Azure AD, ръчно премахнете обекта сираци с помощта на един от следните модули на Azure Active Directory за кратки команди на Windows PowerShell:

    Премествам-MsolContact  
    Премествам-MsolGroup  
    Премествам-MsolUser

    Например за да премахнете осиротели потребителски ИД на john.smith@contoso.com, който първоначално е създаден с помощта на синхронизиране на справочен указател, изпълнете кратката команда:

    Remove-MsolUser-UserPrincipalName John.Smith@Contoso.com