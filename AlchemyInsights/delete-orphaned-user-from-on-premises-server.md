---
title: Изтриване на осиротели потребител от локалния сървър
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/20/2020
ms.locfileid: "45197821"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Изтриване на осиротели потребител от локалния сървър

За да премахнете загубен потребител, изпълнете следните стъпки:

1. Сила на указатели, като следвате инструкциите в [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. За да проверите синхронизирането на директории, вижте [Какво е хибридна самоличност с Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ако синхронизиране функционира правилно, но изтриване на active Directory обект не се разпространява azure AD, ръчно премахнете очесящи обект чрез един от следните Azure Active Directory модул за кратки команди на Windows PowerShell:

    Премахване на MsolConContact  
    Премахване на MsolGroup  
    Премахване на MsolUser

    Например да премахнете осиротели потребителски ИД john.smith@contoso.com, първоначално създаден чрез синхронизиране на директории, изпълнете команда:

    Премахване на MsolUser – UserPrincipalName John.Smith@Contoso.com