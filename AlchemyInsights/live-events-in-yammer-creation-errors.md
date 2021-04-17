---
title: Грешки при създаването на събития на живо в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 383943d670c935403fb7f4466a72474120e27e7a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825504"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="c0b86-102">Грешки при създаването на събития на живо в Yammer</span><span class="sxs-lookup"><span data-stu-id="c0b86-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="c0b86-103">**Създаване на събитие на живо в Yammer**</span><span class="sxs-lookup"><span data-stu-id="c0b86-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="c0b86-104">Yammer винаги ще показва опцията за създаване на събитие на живо.</span><span class="sxs-lookup"><span data-stu-id="c0b86-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="c0b86-105">В някои случаи е възможно потребителят да не отговаря на предварителните условия за създаване на събитие на живо и да получи грешка, когато се опита да го създаде.</span><span class="sxs-lookup"><span data-stu-id="c0b86-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="c0b86-106">Елементите по-долу обхващат често срещани причини за този проблем и предоставят начини за отстраняването му за крайните потребители.</span><span class="sxs-lookup"><span data-stu-id="c0b86-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="c0b86-107">**Кой може да създава събития на живо**</span><span class="sxs-lookup"><span data-stu-id="c0b86-107">**Who can create live events**</span></span>
- <span data-ttu-id="c0b86-108">Лиценз за Office 365 Enterprise E1, E3 или E5 или лиценз за Office 365 A3 или A5.</span><span class="sxs-lookup"><span data-stu-id="c0b86-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="c0b86-109">Разрешение за създаване на събития на живо в центъра за администриране на Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="c0b86-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="c0b86-110">Разрешение за създаване на събития на живо в Microsoft Stream (за събития, които са продуцирани чрез външно приложение или устройство за излъчване).</span><span class="sxs-lookup"><span data-stu-id="c0b86-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="c0b86-111">Пълноправно членство в екипа в организацията (не като гост или от друга организация).</span><span class="sxs-lookup"><span data-stu-id="c0b86-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="c0b86-112">Планиране на частни събрания, споделяне на екрана и споделяне на IP видео, включено в правилата за събрания на Teams.</span><span class="sxs-lookup"><span data-stu-id="c0b86-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="c0b86-113">**Правила за създаване на събития на живо**</span><span class="sxs-lookup"><span data-stu-id="c0b86-113">**Live event creation policies**</span></span>

<span data-ttu-id="c0b86-114">Yammer следва правилата за събития на живо, зададени във вашия клиент на Office 365 за Stream.</span><span class="sxs-lookup"><span data-stu-id="c0b86-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="c0b86-115">По подразбиране всеки във вашата организация може да създаде събитие на живо.</span><span class="sxs-lookup"><span data-stu-id="c0b86-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="c0b86-116">Администраторите могат да [направят промени в тази настройка, което може да попречи на потребителите да създадат събитие на живо](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="c0b86-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="c0b86-117">Важно е да проверите дали потребителите имат разрешения за създаване на събития на живо, ако получат грешка относно правилата.</span><span class="sxs-lookup"><span data-stu-id="c0b86-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
