---
title: Правилата за съхранение в центъра за администриране на Exchange не работят
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952217"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="2d119-102">Правила за съхранение в центъра за администриране на Exchange</span><span class="sxs-lookup"><span data-stu-id="2d119-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="2d119-103">Ако искате да изпълняваме автоматизирани проверки за настройките, споменати по-долу, изберете бутона назад < – в горната част на тази страница и след това въведете имейл адреса на потребителя, който има проблеми с правилата за съхранение.</span><span class="sxs-lookup"><span data-stu-id="2d119-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="2d119-104">Ако имате проблеми с правилата за съхранение в центъра за администриране на Exchange, които не се прилагат към пощенски кутии или елементи, които не се преместват в архивната пощенска кутия, проверете следното:</span><span class="sxs-lookup"><span data-stu-id="2d119-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="2d119-105">**Главни причини:**</span><span class="sxs-lookup"><span data-stu-id="2d119-105">**Root Causes:**</span></span>

- <span data-ttu-id="2d119-106">**Помощникът за управлявани** папки не е обработил пощенската кутия на потребителя.</span><span class="sxs-lookup"><span data-stu-id="2d119-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="2d119-107">Помощникът за управлявани папки се опитва да обработи всяка пощенска кутия във вашата организация, базирана на облака, веднъж на всеки седем дни.</span><span class="sxs-lookup"><span data-stu-id="2d119-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="2d119-108">**Решение:** Изпълнете помощника за управлявани папки.</span><span class="sxs-lookup"><span data-stu-id="2d119-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="2d119-109">**ЗадържанеТо е** разрешено **в** пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="2d119-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="2d119-110">Ако пощенската кутия е поставена в задържанеHold, правилата за съхранение в пощенската кутия няма да бъдат обработвани през това време.</span><span class="sxs-lookup"><span data-stu-id="2d119-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="2d119-111">**Решение:** Проверете състоянието на настройката за задържане на задържането и актуализирайте, ако е необходимо.</span><span class="sxs-lookup"><span data-stu-id="2d119-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="2d119-112">За подробности вижте Задържане [на пощенската кутия.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="2d119-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="2d119-113">**Забележка:** Ако пощенската кутия е по-малка от 10 МБ, помощникът за управлявани папки няма да обработи автоматично пощенската кутия.</span><span class="sxs-lookup"><span data-stu-id="2d119-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="2d119-114">За повече информация относно правилата за съхранение в центъра за администриране на Exchange вижте:</span><span class="sxs-lookup"><span data-stu-id="2d119-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="2d119-115">Етикети за съхранение и правила за съхранение</span><span class="sxs-lookup"><span data-stu-id="2d119-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="2d119-116">[Прилагане на правила за съхранение към пощенски кутии или](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Добавяне или премахване на етикети за [съхранение](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="2d119-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="2d119-117">Как да идентифицирате типа задържане, поставено в пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="2d119-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
