---
title: Проверка за препращане на адреси в пощенски кутии
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481077"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c2266-102">Проверка за препращане на адреси в пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="c2266-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c2266-103">Понякога хакерите препращат имейл съобщения на потребителите към себе си, така че първо ще проверим за препращане на адреси и правила за пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="c2266-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c2266-104">След това ще проверим регистрационните файлове за проверка.</span><span class="sxs-lookup"><span data-stu-id="c2266-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c2266-105">Ето как да проверите за препращащи адреси:</span><span class="sxs-lookup"><span data-stu-id="c2266-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c2266-106">Изберете **потребители**  >  **активни потребители**.</span><span class="sxs-lookup"><span data-stu-id="c2266-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c2266-107">Изберете потребителя, чийто акаунт е компрометиран.</span><span class="sxs-lookup"><span data-stu-id="c2266-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c2266-108">В изплаващо, който се появява, разгънете **Настройки на поща** и след това щракнете върху **Редактиране** за **Препращане на имейл**.</span><span class="sxs-lookup"><span data-stu-id="c2266-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c2266-109">Премахнете всички препращащи адреси, които не разпознавате.</span><span class="sxs-lookup"><span data-stu-id="c2266-109">Remove any forwarding addresses you don't recognize.</span></span>