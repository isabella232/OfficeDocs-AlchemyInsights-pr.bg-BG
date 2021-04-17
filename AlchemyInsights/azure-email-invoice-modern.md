---
title: Модерно фактуриране на имейл в Azure
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820815"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="cc3d6-102">Фактуриране по имейл на Azure</span><span class="sxs-lookup"><span data-stu-id="cc3d6-102">Email invoicing in Azure</span></span>

<span data-ttu-id="cc3d6-103">Трябва да имате роля на собственик или сътрудник в профила за фактуриране или неговия акаунт за фактуриране, за да актуализирате предпочитанието за имейл фактура.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="cc3d6-104">След като сте се включили, всички потребители с роли на собственик, сътрудник, читатели и диспечер на фактури в профил за фактуриране ще получават фактурата си в имейл.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="cc3d6-105">Влезте в портала [Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cc3d6-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="cc3d6-106">Търсене в **Управление на разходите + Фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="cc3d6-107">Изберете **Фактури** от лявата страна и след това изберете **Имейл фактура** от горния край на страницата.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="cc3d6-108">Ако имате няколко профила за фактуриране, изберете профил за фактуриране и след това изберете **Влизане**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="cc3d6-109">Изберете **Актуализиране**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-109">Select **Update**.</span></span>
6. <span data-ttu-id="cc3d6-110">Ако имате няколко профила за фактуриране, изберете профил за фактуриране и след това изберете **Влизане**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="cc3d6-111">Давате на другите достъп да преглеждат, изтеглят и плащат фактури, като им давате ролята "диспечер на фактура" за MCA или MPA профил за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="cc3d6-112">Ако сте избрали да получавате фактурата си по имейл, потребителите също така получават фактурите по имейл.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="cc3d6-113">Влезте в портала [Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="cc3d6-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="cc3d6-114">Търсене в **Управление на разходите + Фактуриране**.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="cc3d6-115">Изберете **Профили за фактуриране** от лявата страна.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="cc3d6-116">От списъка с профили за фактуриране изберете профил за фактуриране, за който искате да дадете роля на диспечер на фактура.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="cc3d6-117">Изберете **Управление на достъпа (IAM)** от лявата страна и след това изберете **Добавяне** от горния край на страницата.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="cc3d6-118">В падащия списък "Роля" изберете **Диспечер на фактура"**".</span><span class="sxs-lookup"><span data-stu-id="cc3d6-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="cc3d6-119">Въведете имейл адреса на потребителя, за да дадете достъп.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="cc3d6-120">Изберете **Записване**, за да дадете ролята.</span><span class="sxs-lookup"><span data-stu-id="cc3d6-120">Select **Save** to assign the role.</span></span>
