---
title: Конфигуриране на точка на свързване на услугата (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034921"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="46692-102">Конфигуриране на точка на свързване на услугата (SCP)</span><span class="sxs-lookup"><span data-stu-id="46692-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="46692-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="46692-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="46692-104">**Причина**: не можете да прочетете SCP обекта и да получите информацията за клиент на Azure ad</span><span class="sxs-lookup"><span data-stu-id="46692-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="46692-105">**Разделителна способност**: прегледайте секцията [Конфигуриране на точка на свързване на услуга](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="46692-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="46692-106">**План за действие**</span><span class="sxs-lookup"><span data-stu-id="46692-106">**Action plan**</span></span>

- <span data-ttu-id="46692-107">Проверете дали устройството е получило GPO за контролираната проверка.</span><span class="sxs-lookup"><span data-stu-id="46692-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="46692-108">Уверете се, че GPO е създал ключове от системния регистър.</span><span class="sxs-lookup"><span data-stu-id="46692-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="46692-109">Уверете се, че имате 2 ключа, създадени със своя ИД на директорията и домейна на домейн onmicrosoft.</span><span class="sxs-lookup"><span data-stu-id="46692-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="46692-110">**Конфигуриране на настройките на системния регистър за клиент за SCP**</span><span class="sxs-lookup"><span data-stu-id="46692-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="46692-111">Използвайте примера по-долу, за да създадете обект с групови правила (GPO), за да разположите настройка на системния регистър, които конфигурират SCP запис в системния регистър на вашите устройства.</span><span class="sxs-lookup"><span data-stu-id="46692-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="46692-112">Отворете конзолата за управление на груповите правила и създайте нов GPO във вашия домейн.</span><span class="sxs-lookup"><span data-stu-id="46692-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="46692-113">Осигурете си новосъздадено име за GPO (например ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="46692-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="46692-114">Редактирайте GPO и намерете следния път: **конфигурацията на компютъра > предпочитания > настройки на Windows > системен регистър**.</span><span class="sxs-lookup"><span data-stu-id="46692-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="46692-115">Щракнете с десния бутон върху **регистратура** и изберете **нов > елемент от системния регистър**.</span><span class="sxs-lookup"><span data-stu-id="46692-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="46692-116">В раздела **Общи** конфигурирайте следното:</span><span class="sxs-lookup"><span data-stu-id="46692-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="46692-117">**Действие**: актуализиране</span><span class="sxs-lookup"><span data-stu-id="46692-117">**Action**: Update</span></span>
    
- <span data-ttu-id="46692-118">**Кошер**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="46692-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="46692-119">**Клавиш път**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="46692-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="46692-120">**Име на стойност**: TenantId</span><span class="sxs-lookup"><span data-stu-id="46692-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="46692-121">**Тип стойност**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="46692-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="46692-122">**Данни за стойност**: GUID или ИД на указателя на вашата инстанция на Azure ad (тази стойност може да бъде намерена в **портала на Azure > azure Active directory > свойства > ИД на директорията**)</span><span class="sxs-lookup"><span data-stu-id="46692-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="46692-123">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="46692-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="46692-124">Щракнете с десния бутон върху **регистратура** и изберете **нов > елемент от системния регистър**.</span><span class="sxs-lookup"><span data-stu-id="46692-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="46692-125">В раздела **Общи** конфигурирайте следното:</span><span class="sxs-lookup"><span data-stu-id="46692-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="46692-126">**Действие**: актуализиране</span><span class="sxs-lookup"><span data-stu-id="46692-126">**Action**: Update</span></span>
    
- <span data-ttu-id="46692-127">**Кошер**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="46692-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="46692-128">**Клавиш път**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="46692-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="46692-129">**Име на стойност**: TenantName</span><span class="sxs-lookup"><span data-stu-id="46692-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="46692-130">**Тип стойност**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="46692-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="46692-131">**Данни за стойност**: вашето потвърдено име на домейн, ако използвате външна среда, като НАПРИМЕР AD FS.</span><span class="sxs-lookup"><span data-stu-id="46692-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="46692-132">Вашите удостоверени имена на домейни или името на вашия домейн в onmicrosoft.com (например contoso. домейн onmicrosoft). com, ако използвате управлявана среда</span><span class="sxs-lookup"><span data-stu-id="46692-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="46692-133">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="46692-133">Click **OK**.</span></span>

7. <span data-ttu-id="46692-134">Затворете редактора за новосъздадения GPO.</span><span class="sxs-lookup"><span data-stu-id="46692-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="46692-135">Свържете новосъздадения GPO до желаното място, където се съдържат домейни, които принадлежат на вашата управлявана популация за внедряване.</span><span class="sxs-lookup"><span data-stu-id="46692-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="46692-136">За повече информация вижте [управление на проверката на хибридно AZURE ad JOIN – AZURE ad | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) и  [отстраняване на неизправности в хибридни Azure Active Directory присъединен устройства | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="46692-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









