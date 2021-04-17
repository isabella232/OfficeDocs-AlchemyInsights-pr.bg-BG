---
title: Собственикът не може да създаде подпапка с помощта на Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836124"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="abeeb-102">Собственикът не може да създаде подпапка с помощта на Outlook</span><span class="sxs-lookup"><span data-stu-id="abeeb-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="abeeb-103">**Има текущ проблем със собствениците на публични папки, които създават подпапки с помощта на Outlook. Проблемът скоро ще бъде коригиран.**</span><span class="sxs-lookup"><span data-stu-id="abeeb-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="abeeb-104">Междувременно използвайте едно от следните заобиколни решения:</span><span class="sxs-lookup"><span data-stu-id="abeeb-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="abeeb-105">Използвайте Outlook for MAC, за да създадете подпапка, тъй като проблемът засяга само Outlook за настолни прозорци (всички версии)</span><span class="sxs-lookup"><span data-stu-id="abeeb-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="abeeb-106">Дайте на администратора да създаде подпапката с помощта на EXO Shell или EAC</span><span class="sxs-lookup"><span data-stu-id="abeeb-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="abeeb-107">Промяна на папката DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя на други пощенски кутии, различни от пощенската кутия за съдържание за папката, която причинява проблем</span><span class="sxs-lookup"><span data-stu-id="abeeb-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="abeeb-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="abeeb-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="abeeb-109">Изчакайте един час, рестартирайте клиента на Outlook</span><span class="sxs-lookup"><span data-stu-id="abeeb-109">Wait for an hour, restart outlook client</span></span>