---
title: Собственик не може да създаде подпапка с помощта на Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665707"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="0e075-102">Собственик не може да създаде подпапка с помощта на Outlook</span><span class="sxs-lookup"><span data-stu-id="0e075-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="0e075-103">**Има текущ проблем с собственици на публични папки, създаващи подпапки с помощта на Outlook. Проблемът ще бъде коригиран скоро.**</span><span class="sxs-lookup"><span data-stu-id="0e075-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="0e075-104">Междувременно Използвайте едно от следните заобиколни решения:</span><span class="sxs-lookup"><span data-stu-id="0e075-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="0e075-105">Използвайте Outlook for MAC, за да създадете подпапката, тъй като проблемът влияе само на Outlook за настолната версия на Windows (всички версии)</span><span class="sxs-lookup"><span data-stu-id="0e075-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="0e075-106">Помолете администратор да създаде подпапката, като използва ЕКСО черупка или EAC</span><span class="sxs-lookup"><span data-stu-id="0e075-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="0e075-107">Промяна на DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя в друга пощенска кутия от пощенската кутия на съдържанието за папката, която създава проблема</span><span class="sxs-lookup"><span data-stu-id="0e075-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="0e075-108">*Set-пощенска кутия user1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="0e075-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="0e075-109">Изчакайте един час, рестартирайте клиент на Outlook</span><span class="sxs-lookup"><span data-stu-id="0e075-109">Wait for an hour, restart outlook client</span></span>