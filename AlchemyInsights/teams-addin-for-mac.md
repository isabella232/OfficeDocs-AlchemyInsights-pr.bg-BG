---
title: Teams добавка за Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582059"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="4aca8-102">Teams добавка за Mac</span><span class="sxs-lookup"><span data-stu-id="4aca8-102">Teams add-in for Mac</span></span>

<span data-ttu-id="4aca8-103">За да отстраните Teams добавка за потребители на операционната система Mac, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="4aca8-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="4aca8-104">**Стъпка 1:** Ако имате хибридно Exchange локално (изисква се 2016 CU3 или по-нова версия), използвайте инструмента Test-HMA.ps1, за да потвърдите, че хибридното модерно удостоверяване е конфигурирано правилно.</span><span class="sxs-lookup"><span data-stu-id="4aca8-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="4aca8-105">За повече информация вижте Проверка [на настройката за модерно хибридно удостоверяване за Outlook за iOS и Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="4aca8-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="4aca8-106">**Забележка** Използвайте формата за UPN адрес (например username@contoso.com [),](mailto:username@contoso.com)а не домейн\потребителско име.</span><span class="sxs-lookup"><span data-stu-id="4aca8-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="4aca8-107">Направете това дори за потребители с Exchange Online пощенски кутии.</span><span class="sxs-lookup"><span data-stu-id="4aca8-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="4aca8-108">**Стъпка 2:** Дайте на потребителя да отиде **в "Акаунти за**  >  **инструменти"**... в Outlook за Mac и намерете и изберете акаунта.</span><span class="sxs-lookup"><span data-stu-id="4aca8-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="4aca8-109">Уверете се, че потребителското име в списъка е във формат UPN [(например username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="4aca8-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="4aca8-110">**Стъпка 3:** Уверете се, че потребителят е лицензиран Microsoft Teams потребител.</span><span class="sxs-lookup"><span data-stu-id="4aca8-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="4aca8-111">Потребителят трябва да използва абонамента за Office 365 Mac, версия на продукта 16.24 или по-нова.</span><span class="sxs-lookup"><span data-stu-id="4aca8-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>