---
title: Създаване на група
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816334"
---
# <a name="create-a-group"></a><span data-ttu-id="320ce-102">Създаване на група</span><span class="sxs-lookup"><span data-stu-id="320ce-102">Create a group</span></span>

<span data-ttu-id="320ce-103">Тази тема описва създаването на групи.</span><span class="sxs-lookup"><span data-stu-id="320ce-103">This topic describes group creation.</span></span>

<span data-ttu-id="320ce-104">**Разрешение за създаване на група**</span><span class="sxs-lookup"><span data-stu-id="320ce-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="320ce-105">Уверете се, че сте упълномощени да създадете нова група.</span><span class="sxs-lookup"><span data-stu-id="320ce-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="320ce-106">Глобалните администратори могат да забраняват създаването на групи в портала на Azure или панела на Access.</span><span class="sxs-lookup"><span data-stu-id="320ce-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="320ce-107">Може да се наложи администратор да създаде новата група за вас или да ви даде подходящи разрешения.</span><span class="sxs-lookup"><span data-stu-id="320ce-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="320ce-108">**Управление на разрешенията за създаване на група**</span><span class="sxs-lookup"><span data-stu-id="320ce-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="320ce-109">Глобалните администратори могат да управляват разрешенията за създаване на групи (от съображения, свързани със защитата) или групите на Office 365, създадени в портала на Azure или панела на Access, като изберат "Потребителите могат да създават групи за защита в портали на Azure" или "Потребителите могат да създават групи на Office 365 в порталите на Azure" във всички групи  >  **Общи (Настройки)**.</span><span class="sxs-lookup"><span data-stu-id="320ce-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="320ce-110">Можете също да ограничите създаването на група, за да изберете група потребители, ако имате лиценз за Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="320ce-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="320ce-111">**Забраняване на известието за добре дошли за новите членове на групата на Office 365**</span><span class="sxs-lookup"><span data-stu-id="320ce-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="320ce-112">Известието за добре дошли, изпратено до потребители, които са добавени към групи на Office 365, може да бъде забранено, като зададете **UnifiedGroupWelcomeMessageEnabled** на False в Powershell.</span><span class="sxs-lookup"><span data-stu-id="320ce-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="320ce-113">Научете повече за тази настройка [тук](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="320ce-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

