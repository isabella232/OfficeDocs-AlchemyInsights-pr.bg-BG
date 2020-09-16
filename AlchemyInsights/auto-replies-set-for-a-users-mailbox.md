---
title: Задаване на автоматични отговори за пощенска кутия
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715118"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="c88b7-102">Задаване на автоматични отговори за пощенска кутия на потребител</span><span class="sxs-lookup"><span data-stu-id="c88b7-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="c88b7-103">**Метод 1**</span><span class="sxs-lookup"><span data-stu-id="c88b7-103">**Method 1**</span></span>

1. <span data-ttu-id="c88b7-104">Влезте в портала на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c88b7-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="c88b7-105">Отидете на **Потребители > Активни потребители** (или **Групи > Споделени пощенски кутии**, ако сте задали това за споделена пощенска кутия).</span><span class="sxs-lookup"><span data-stu-id="c88b7-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="c88b7-106">Изберете потребител с пощенска кутия на Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="c88b7-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="c88b7-107">В падащото меню отдясно отидете на **Настройки за поща > Автоматични отговори** (ако това е споделена пощенска кутия, просто щракнете върху **Автоматични отговори** в падащото меню).</span><span class="sxs-lookup"><span data-stu-id="c88b7-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="c88b7-108">**Метод 2**</span><span class="sxs-lookup"><span data-stu-id="c88b7-108">**Method 2**</span></span>

1. <span data-ttu-id="c88b7-109">Влезте в портала за администриране на Microsoft 365, като използвате идентификационни данни на администратор.</span><span class="sxs-lookup"><span data-stu-id="c88b7-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="c88b7-110">Разгънете **Центрове за администриране** и след това щракнете върху **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="c88b7-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="c88b7-111">Щракнете върху картината в горния десен ъгъл, щракнете върху **Друг потребител** и след това изберете пощенската кутия на потребителя, която искате да промените.</span><span class="sxs-lookup"><span data-stu-id="c88b7-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="c88b7-112">В лявата част, изберете \*\*Опции \*\*, щракнете върху **Организиране на имейл**, след което щракнете върху **Автоматични отговори.**</span><span class="sxs-lookup"><span data-stu-id="c88b7-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="c88b7-113">**Метод 3**</span><span class="sxs-lookup"><span data-stu-id="c88b7-113">**Method 3**</span></span>

<span data-ttu-id="c88b7-114">Изпълнете следната кратка команда в PowerShell за Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="c88b7-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="c88b7-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="c88b7-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="c88b7-116">За повече информация за тази кратка команда вижте [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="c88b7-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
