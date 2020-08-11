---
title: Добавка за Teams за Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629379"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="2d884-102">Добавка за Teams за Mac</span><span class="sxs-lookup"><span data-stu-id="2d884-102">Teams add-in for Mac</span></span>

<span data-ttu-id="2d884-103">За да отстраните добавка за липсващи екипи за потребители на операционна система Mac, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="2d884-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="2d884-104">**Стъпка 1:** Ако имате хибридно разполагане на Exchange (2016 CU3 или по-нова версия), използвайте инструмента за Test-HMA.ps1, за да потвърдите, че хибридното модерно удостоверяване е конфигурирано правилно.</span><span class="sxs-lookup"><span data-stu-id="2d884-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="2d884-105">За повече информация вижте [проверка на хибридно модерно удостоверяване за Outlook за IOS и Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="2d884-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="2d884-106">**Забележка** Използвайте формата UPN адрес (например [username@contoso.com](mailto:username@contoso.com)), а не domain\username.</span><span class="sxs-lookup"><span data-stu-id="2d884-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="2d884-107">Направете това дори за потребители с пощенски кутии на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="2d884-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="2d884-108">**Стъпка 2:** Помолете потребителя да премине към **инструменти**за  >  **акаунти**... в Outlook for Mac и намерете и изберете акаунта.</span><span class="sxs-lookup"><span data-stu-id="2d884-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="2d884-109">Уверете се, че потребителското име в списъка е в UPN формат (например [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="2d884-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="2d884-110">**Стъпка 3:** Уверете се, че потребителят е лицензиран потребител на Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2d884-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="2d884-111">Потребителят трябва да използва абонамента за Office 365 for Mac, версия на продукта 16,24 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="2d884-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>