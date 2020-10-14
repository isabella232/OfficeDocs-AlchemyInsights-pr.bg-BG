---
title: Публична папка "Изпращане като разрешена поща" в ЕКСО
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461751"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="eb292-102">Публична папка за разрешена поща в SendAs</span><span class="sxs-lookup"><span data-stu-id="eb292-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="eb292-103">Следващият пример присвоява разрешения за "Изпращане като" за публичната папка на NewPF1, за да позволите на потребителя Jason.</span><span class="sxs-lookup"><span data-stu-id="eb292-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="eb292-104">Add-RecipientPermission самоличност "NewPF1" – попечител "Jason" – AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="eb292-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="eb292-105">За подробен синтаксис и информация за параметрите вижте даване [на разрешения за "Изпращане като" или "Изпращане от името" за публични папки с активиран имейл](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="eb292-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

