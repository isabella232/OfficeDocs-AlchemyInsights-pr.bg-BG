---
title: Защита от фалшиви Attack
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034911"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="81529-102">Защита от фалшиви Attack</span><span class="sxs-lookup"><span data-stu-id="81529-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="81529-103">Фалшиви е недоставящи отчети (известни също като недоставяне или върнати съобщения), които получавате за съобщения, които не сте изпратили.</span><span class="sxs-lookup"><span data-stu-id="81529-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="81529-104">Spammers Forge (пародия) The **from:** адресът на техните съобщения, и те често използват реални имейл адреси, за да подадат доверието към своите съобщения.</span><span class="sxs-lookup"><span data-stu-id="81529-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="81529-105">Така че, когато подателите на нежелана поща неизбежно изпращат съобщения до несъществуващи получатели, имейл сървърът местоназначение е подмамен да върне недоставяното съобщение в NDR до подкования подател в адреса **from:** .</span><span class="sxs-lookup"><span data-stu-id="81529-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="81529-106">Допълнителна информация можете да намерите в [фалшиви в EoP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="81529-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="81529-107">**Разрешаване на защита на фалшиви**</span><span class="sxs-lookup"><span data-stu-id="81529-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="81529-108">За да разрешите защитата на фалшиви, следвайте пътя по-долу.</span><span class="sxs-lookup"><span data-stu-id="81529-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="81529-109">**protection.office.com > > политика за управление на заплахите > антиспам > изберете правилата за филтриране на нежелана поща и правила за редактиране на > за нежелана поща > Маркирай като нежелана поща > NDR фалшиви, за да го зададете на "вкл."**</span><span class="sxs-lookup"><span data-stu-id="81529-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="81529-110">Ако смятате, че даден акаунт е компрометиран, вижте следното:</span><span class="sxs-lookup"><span data-stu-id="81529-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="81529-111">Отговаряне на компрометиран имейл акаунт</span><span class="sxs-lookup"><span data-stu-id="81529-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="81529-112">Премахване на блокирани потребители от портала за ограничени потребители в Office 365</span><span class="sxs-lookup"><span data-stu-id="81529-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



