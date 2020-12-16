---
title: Услуги за прехвърляне – преместване на всички услуги на RDFE към друг абонамент
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691929"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="381db-102">Услуги за прехвърляне – преместване на всички услуги на RDFE към друг абонамент</span><span class="sxs-lookup"><span data-stu-id="381db-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="381db-103">**"Премахни ресурсите"**</span><span class="sxs-lookup"><span data-stu-id="381db-103">**Move resources**</span></span>

<span data-ttu-id="381db-104">Ресурсите на Azure могат да бъдат преместени към друг абонамент за Azure или група ресурси под един и същ абонамент чрез Azure Portal, Azure PowerShell, Azure CLI или останалата част от API за преместване на ресурси.</span><span class="sxs-lookup"><span data-stu-id="381db-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="381db-105">За да можете да прехвърлите ресурси, вижте:</span><span class="sxs-lookup"><span data-stu-id="381db-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="381db-106">Контролен списък, преди да преместите ресурсите</span><span class="sxs-lookup"><span data-stu-id="381db-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="381db-107">Услуги, които могат да бъдат преместени</span><span class="sxs-lookup"><span data-stu-id="381db-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="381db-108">Как се проверява движението</span><span class="sxs-lookup"><span data-stu-id="381db-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="381db-109">Ръководство за движение за услуги</span><span class="sxs-lookup"><span data-stu-id="381db-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="381db-110">За да премествате съществуващи ресурси към друга група ресурси или абонамент, можете да използвате:</span><span class="sxs-lookup"><span data-stu-id="381db-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="381db-111">Портал на Azure</span><span class="sxs-lookup"><span data-stu-id="381db-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="381db-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="381db-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="381db-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="381db-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="381db-114">REST API</span><span class="sxs-lookup"><span data-stu-id="381db-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="381db-115">Урок: [премествате ресурси на Azure към друга група ресурси или абонамент](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="381db-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="381db-116">**Отстраняване на грешки при диспечера за ресурси на Azure**</span><span class="sxs-lookup"><span data-stu-id="381db-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="381db-117">Вижте статиите по-долу, за да научите за някои често срещани грешки при разполагане на Azure и да получите информация за отстраняването им.</span><span class="sxs-lookup"><span data-stu-id="381db-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="381db-118">Ако не можете да намерите кода на грешката за грешката си за разполагане, вижте [намиране на код на грешка](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="381db-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="381db-119">Отстраняване на грешки при разполагане</span><span class="sxs-lookup"><span data-stu-id="381db-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="381db-120">Отстраняване на неизправности при преместване на ресурси на Azure към нова група ресурси или абонамент</span><span class="sxs-lookup"><span data-stu-id="381db-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="381db-121">Имайте предвид, че ако искате да надстроите своя абонамент за Azure, като например да преминете от свободен към платено, ще трябва да конвертирате абонамента си.</span><span class="sxs-lookup"><span data-stu-id="381db-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="381db-122">За да надстроите безплатно изпробване, вижте [надстройване на вашия безплатен пробен период или абонамент за Microsoft за Azure, за да можете да плащате по-нататък](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="381db-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="381db-123">За да промените акаунт за плащане като за отиване, вижте [Промяна на вашия абонамент за вашия Azure Pay-do-Go за друго предложение](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="381db-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="381db-124">**За да добавите или свържете абонамент за Azure към вашия клиент на Azure Active Directory:**</span><span class="sxs-lookup"><span data-stu-id="381db-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="381db-125">Впишете се и изберете абонамента, който искате да използвате, от страницата ' ' рецепти ' ' [в портала на Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="381db-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="381db-126">Изберете **Промяна на справочен указател**.</span><span class="sxs-lookup"><span data-stu-id="381db-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="381db-127">Прегледайте всички предупреждения, които се появяват, след което изберете **Промяна**.</span><span class="sxs-lookup"><span data-stu-id="381db-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="381db-128">Справочникът се променя за абонамента и ще получите съобщение за успех.</span><span class="sxs-lookup"><span data-stu-id="381db-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="381db-129">Използвайте превключвателя *Directory* , за да отидете в новия си указател.</span><span class="sxs-lookup"><span data-stu-id="381db-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="381db-130">Възможно е да са необходими до 10 минути, за да се покаже всичко правилно.</span><span class="sxs-lookup"><span data-stu-id="381db-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="381db-131">**Препоръчвани документи**</span><span class="sxs-lookup"><span data-stu-id="381db-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="381db-132">Прехвърляне на собствеността върху абонамент за Azure</span><span class="sxs-lookup"><span data-stu-id="381db-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="381db-133">Преминаване на ресурси към нова група ресурси или абонамент</span><span class="sxs-lookup"><span data-stu-id="381db-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="381db-134">Управление на ресурси чрез портала на Azure</span><span class="sxs-lookup"><span data-stu-id="381db-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
