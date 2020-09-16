---
title: Множество обекти имат един и същ имейл адрес като самоличност
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724604"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="0c93a-102">Множество обекти имат един и същ имейл адрес като самоличност</span><span class="sxs-lookup"><span data-stu-id="0c93a-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="0c93a-103">**Множество обекти**</span><span class="sxs-lookup"><span data-stu-id="0c93a-103">**Multiple objects**</span></span>

<span data-ttu-id="0c93a-104">Една от често срещаните причини за тази грешка не е в състояние да маршрутизира правилно заявка на Outlook Web Access в наличност на множество обекти, които имат един и същ имейл адрес като самоличност.</span><span class="sxs-lookup"><span data-stu-id="0c93a-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="0c93a-105">За да намерите тези обекти, изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="0c93a-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="0c93a-106">· Получаване на получателя <email address></span><span class="sxs-lookup"><span data-stu-id="0c93a-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="0c93a-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="0c93a-107">· Get-User <email address></span></span>

<span data-ttu-id="0c93a-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="0c93a-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="0c93a-109">· Свържете се с нас <email address></span><span class="sxs-lookup"><span data-stu-id="0c93a-109">· Get-Contact <email address></span></span>

<span data-ttu-id="0c93a-110">· Получаване на пощенска кутия <email address> – PublicFolder</span><span class="sxs-lookup"><span data-stu-id="0c93a-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="0c93a-111">· Получаване на пощенска кутия <email address> – IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="0c93a-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="0c93a-112">· Получаване на пощенска кутия <email address> – InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="0c93a-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="0c93a-113">За да отстраните проблема, премахнете множество обекти с една и съща самоличност на имейл и се уверете, че има един обект с конкретната самоличност за имейл и че неговият тип получател е UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="0c93a-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="0c93a-114">**Един и същ адрес се използва за пощенските кутии за фирми и потребители**</span><span class="sxs-lookup"><span data-stu-id="0c93a-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="0c93a-115">Друга причина е, когато един и същ адрес се използва за пощенски кутии за фирми и потребители.</span><span class="sxs-lookup"><span data-stu-id="0c93a-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="0c93a-116">В този случай потребителят трябва да промени своя първичен псевдоним за потребител, докато Cafe не подкрепи този сценарий.</span><span class="sxs-lookup"><span data-stu-id="0c93a-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="0c93a-117">Това е постоянна грешка, която не изчезва без интервенция.</span><span class="sxs-lookup"><span data-stu-id="0c93a-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="0c93a-118">За подробности вижте [Промяна на имейл адреса или телефонния номер за вашия акаунт в Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="0c93a-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>