---
title: Няма достъп до публични папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959484"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="0a27b-102">Outlook не може да се свърже с публични папки</span><span class="sxs-lookup"><span data-stu-id="0a27b-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="0a27b-103">Ако достъп до публична папка не работи за няколко потребители, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="0a27b-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="0a27b-104">Свързване с ЕКЗО PowerShell и Конфигурирайте пощенската кутия на проблема по подразбиране на проблемния потребителски акаунт да съвпада с един на работен потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="0a27b-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="0a27b-105">Пример:</span><span class="sxs-lookup"><span data-stu-id="0a27b-105">Example:</span></span>

<span data-ttu-id="0a27b-106">Get-пощенска кутия WorkingUser | Пощенска кутия, ефективна пощенска кутия за Подразбираннопубликуване</span><span class="sxs-lookup"><span data-stu-id="0a27b-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="0a27b-107">Set-пощенска кутия Проблемпотребител-Подразбиранепублична пощенска кутия \<стойност от предишната команда></span><span class="sxs-lookup"><span data-stu-id="0a27b-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="0a27b-108">Изчакайте поне един час, за да влезе в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="0a27b-108">Wait at least one hour for the change to take effect.</span></span>