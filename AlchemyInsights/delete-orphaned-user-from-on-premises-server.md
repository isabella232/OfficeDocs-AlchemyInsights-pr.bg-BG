---
title: Изтриване на осиротели потребители от локалния сървър
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
ms.openlocfilehash: a6af617fa4235868f0754ff4c06f4cc73b1700ef14ea449dd1886ab100ddd384
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102229"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Изтриване на осиротели потребители от локалния сървър

За да премахнете осиротели потребители, изпълнете следните стъпки:

1. Принудително синхронизиране на справочника, като следвате инструкциите в Какво е [хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. За да проверите синхронизирането на [справочника, вижте Какво представлява хибридната самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ако синхронизирането функционира правилно, но изтриването на обекти на Active Directory не се разпространява в Azure AD, премахнете ръчно сирацирания обект с помощта на един от следните кратки команди на Azure Active Directory на Windows PowerShell:

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    Например за да премахнете загубени потребителски ИД john.smith@contoso.com, създадени първоначално с помощта на синхронизирането на справочника, изпълнете кратката команда:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com