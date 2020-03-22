---
title: Публични папки не могат да бъдат достъпни
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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891738"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="0f0d3-102">Outlook не може да се свърже с публични папки</span><span class="sxs-lookup"><span data-stu-id="0f0d3-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="0f0d3-103">Ако достъпът до публична папка не работи за някои потребители, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="0f0d3-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="0f0d3-104">Свързване с EXO PowerShell и конфигуриране на параметъра DefaultPublicFolderMailbox на потребителския акаунт на проблема да съответства на параметъра на работещ потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="0f0d3-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="0f0d3-105">Пример:</span><span class="sxs-lookup"><span data-stu-id="0f0d3-105">Example:</span></span>

<span data-ttu-id="0f0d3-106">Потребител на работа с пощенски кутии | фута по подразбиранеПубличнапапка,ефективнапубличнапапкаПощенска кутия</span><span class="sxs-lookup"><span data-stu-id="0f0d3-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="0f0d3-107">Задаване на пощенска кутия за \<проблемПотребител -DefaultPublicFolderMailbox стойност от предишна команда></span><span class="sxs-lookup"><span data-stu-id="0f0d3-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="0f0d3-108">Изчакайте поне един час, за да влязат в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="0f0d3-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="0f0d3-109">Ако проблемът остава, моля, следвайте [тази процедура](https://aka.ms/pfcte) за отстраняване на проблеми с публична папка достъп с помощта на Outlook.</span><span class="sxs-lookup"><span data-stu-id="0f0d3-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>