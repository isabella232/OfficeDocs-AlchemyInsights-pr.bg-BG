---
title: Създаване на група
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088519"
---
# <a name="create-a-group"></a><span data-ttu-id="4d2d1-102">Създаване на група</span><span class="sxs-lookup"><span data-stu-id="4d2d1-102">Create a group</span></span>

<span data-ttu-id="4d2d1-103">Тази тема описва създаването на групи.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-103">This topic describes group creation.</span></span>

<span data-ttu-id="4d2d1-104">**Разрешение за създаване на група**</span><span class="sxs-lookup"><span data-stu-id="4d2d1-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="4d2d1-105">Уверете се, че сте упълномощени да създавате нова група.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="4d2d1-106">Глобалните администратори могат да забранят създаването на групи в портала на Azure или панела на Access.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="4d2d1-107">Може да ви е нужен администратор, за да създадете новата група вместо вас или за да ви бъдат дадени подходящи разрешения.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="4d2d1-108">**Управление на разрешения за създаване на група**</span><span class="sxs-lookup"><span data-stu-id="4d2d1-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="4d2d1-109">Глобалните администратори могат да управляват разрешенията за създаване на групи (за свързани със защитата причини) или групи на Office 365, създадени в портала на Azure или **панела на Access**, като изберете "потребители могат да създадат групи за защита в Azure Portals" или "потребителите могат да създават групи на Office 365 в Azure Portals"  >  **General (Settings)**</span><span class="sxs-lookup"><span data-stu-id="4d2d1-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="4d2d1-110">Можете също да ограничите създаването на групи, за да изберете група от потребители, ако имате лиценз за Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="4d2d1-111">**Забраняване на добре дошли уведомявания за нови членове на групата на Office 365**</span><span class="sxs-lookup"><span data-stu-id="4d2d1-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="4d2d1-112">Известието за добре дошли, изпратено до потребители, които са добавени към групите на Office 365, могат да бъдат забранени чрез задаване на **UnifiedGroupWelcomeMessageEnabled** на FALSE в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4d2d1-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="4d2d1-113">Запознайте се с тази настройка [тук](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="4d2d1-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

