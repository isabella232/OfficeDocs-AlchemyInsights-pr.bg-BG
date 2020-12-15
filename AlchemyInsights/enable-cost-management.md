---
title: Разрешаване на управлението на разходите
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676827"
---
# <a name="enable-cost-management"></a><span data-ttu-id="11fff-102">Разрешаване на управлението на разходите</span><span class="sxs-lookup"><span data-stu-id="11fff-102">Enable cost management</span></span>

<span data-ttu-id="11fff-103">**Какво означават разходите за вашата организация?**</span><span class="sxs-lookup"><span data-stu-id="11fff-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="11fff-104">Организациите, използващи акаунти за корпоративно споразумение (EA) или споразумение за клиенти на Microsoft (МСА), могат да забранят достъпа до информацията за разходите и ценовата информация.</span><span class="sxs-lookup"><span data-stu-id="11fff-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="11fff-105">След като влезете в портала на Azure, той може да използва API за фактуриране, за да получи по програмен път фактури (след като сте се записали) и подробности за използването.</span><span class="sxs-lookup"><span data-stu-id="11fff-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="11fff-106">**Как да разрешите на допълнителни потребители да имат достъп до фактури**</span><span class="sxs-lookup"><span data-stu-id="11fff-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="11fff-107">Отидете на " **абонаменти" Блейд** в портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="11fff-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="11fff-108">Изберете **фактури** и след това **достъп до фактури**.</span><span class="sxs-lookup"><span data-stu-id="11fff-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="11fff-109">Включване на Access, последвано от записване на промените, за да разрешите на потребителите в обхватните роли за абонаменти да изтеглят фактури.</span><span class="sxs-lookup"><span data-stu-id="11fff-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="11fff-110">Администраторът на акаунта може също да конфигурира да има фактури, изпратени по имейл.</span><span class="sxs-lookup"><span data-stu-id="11fff-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="11fff-111">За да научите повече, вижте [получаване на фактурата ви по имейл](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="11fff-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="11fff-112">**Как се добавят потребители към ролята на четящия четец**</span><span class="sxs-lookup"><span data-stu-id="11fff-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="11fff-113">Отидете на " **абонаменти" Блейд** в портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="11fff-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="11fff-114">Изберете **контрол на достъпа (IAM)** и след това щракнете върху **Добави**.</span><span class="sxs-lookup"><span data-stu-id="11fff-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="11fff-115">Изберете **Reader за фактуриране** в страницата **Изберете роля** .</span><span class="sxs-lookup"><span data-stu-id="11fff-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="11fff-116">Въведете имейла на потребителя, когото искате да поканите, и след това щракнете върху **OK** , за да изпратите поканата.</span><span class="sxs-lookup"><span data-stu-id="11fff-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="11fff-117">Следвайте инструкциите, предоставени в имейла за Поканване, за да влезете като четец за фактуриране.</span><span class="sxs-lookup"><span data-stu-id="11fff-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="11fff-118">За повече информация вижте [предоставяне на достъп до фактуриране](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="11fff-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="11fff-119">**Препоръчвани документи**</span><span class="sxs-lookup"><span data-stu-id="11fff-119">**Recommended documents**</span></span>

- [<span data-ttu-id="11fff-120">Разрешаване на изгледи на DA и AO чрез портала на EA</span><span class="sxs-lookup"><span data-stu-id="11fff-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="11fff-121">Разходи, включени в управлението на разходите</span><span class="sxs-lookup"><span data-stu-id="11fff-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="11fff-122">Поддържани предложения на Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="11fff-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="11fff-123">Преглед на разходите в анализа на разходите</span><span class="sxs-lookup"><span data-stu-id="11fff-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="11fff-124">Предоставяне на достъп до информацията за фактуриране</span><span class="sxs-lookup"><span data-stu-id="11fff-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="11fff-125">Проверяване на достъпа до клиентско споразумение на Microsoft</span><span class="sxs-lookup"><span data-stu-id="11fff-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






