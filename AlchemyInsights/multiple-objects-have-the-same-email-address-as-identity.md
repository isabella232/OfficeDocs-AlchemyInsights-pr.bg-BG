---
title: Множество обекти имат същия имейл адрес като идентичност
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438735"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="9463f-102">Множество обекти имат същия имейл адрес като идентичност</span><span class="sxs-lookup"><span data-stu-id="9463f-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="9463f-103">**Множество обекти**</span><span class="sxs-lookup"><span data-stu-id="9463f-103">**Multiple objects**</span></span>

<span data-ttu-id="9463f-104">Една от най-честите причини за тази грешка е да не можете да маршрутите outlook Web Access заявка правилно в присъствието на множество обекти, които имат същия имейл адрес като самоличност.</span><span class="sxs-lookup"><span data-stu-id="9463f-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="9463f-105">За да намерите тези обекти, изпълнете следните команди:</span><span class="sxs-lookup"><span data-stu-id="9463f-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="9463f-106">· Получаване на получател<email address></span><span class="sxs-lookup"><span data-stu-id="9463f-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="9463f-107">· Потребител за получаване<email address></span><span class="sxs-lookup"><span data-stu-id="9463f-107">· Get-User <email address></span></span>

<span data-ttu-id="9463f-108">· Потребител <email address> - Софтуерен Потребител</span><span class="sxs-lookup"><span data-stu-id="9463f-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="9463f-109">· Контакт с вас<email address></span><span class="sxs-lookup"><span data-stu-id="9463f-109">· Get-Contact <email address></span></span>

<span data-ttu-id="9463f-110">· Get-пощенска кутия <email address> publicFolder</span><span class="sxs-lookup"><span data-stu-id="9463f-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="9463f-111">· Пощенска кутия <email address> -IncludeSoftИзтрешенmailbox</span><span class="sxs-lookup"><span data-stu-id="9463f-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="9463f-112">· Пощенска кутия <email address> - неактивни само</span><span class="sxs-lookup"><span data-stu-id="9463f-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="9463f-113">За да разрешите проблема, премахнете няколко обекта с една и съща самоличност на имейл и се уверете, че има един обект с конкретен имейл самоличността и че типа на получателя е UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="9463f-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="9463f-114">**Същият адрес се използва за пощенски кутии за фирми и потребители**</span><span class="sxs-lookup"><span data-stu-id="9463f-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="9463f-115">Друга причина е, когато се използва същия адрес за бизнес и потребителски пощенски кутии.</span><span class="sxs-lookup"><span data-stu-id="9463f-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="9463f-116">В този случай потребителят трябва да промените основния потребителски псевдоним, докато кафе поддържа този сценарий.</span><span class="sxs-lookup"><span data-stu-id="9463f-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="9463f-117">Това е постоянна грешка, която не изчезва без намеса.</span><span class="sxs-lookup"><span data-stu-id="9463f-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="9463f-118">За подробности вижте [Промяна на имейл адреса или телефонния номер за вашия акаунт в Microsoft](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="9463f-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>