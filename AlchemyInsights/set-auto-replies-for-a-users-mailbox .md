---
title: Задаване на автоматични отговори за пощенска кутия на потребител
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506406"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>Задаване на автоматични отговори за пощенска кутия на потребител

**Метод 1**

1. Влезте в портала на Office 365.

2. Отидете на **Потребители > Активни потребители** (или **Групи > Споделени пощенски кутии**, ако сте задали това за споделена пощенска кутия).

3. Изберете потребител с пощенска кутия на Microsoft Exchange.

4. В падащото меню отдясно отидете на **Настройки за поща > Автоматични отговори** (ако това е споделена пощенска кутия, просто щракнете върху **Автоматични отговори** в падащото меню).

**Метод 2**

1. Влезте в портала за администриране на Office 365, като използвате идентификационни данни на администратор.

2. Разгънете **Центрове за администриране** и след това щракнете върху **Exchange**.

3. Щракнете върху картината в горния десен ъгъл, щракнете върху **Друг потребител** и след това изберете пощенската кутия на потребителя, която искате да промените.

4. В лявата част, изберете **Опции **, щракнете върху **Организиране на имейл**, след което щракнете върху **Автоматични отговори.**

**Метод 3**

Изпълнете следната кратка команда в PowerShell за Exchange Online:

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

За повече информация за тази кратка команда вижте [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).
