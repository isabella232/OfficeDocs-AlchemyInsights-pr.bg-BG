---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499371"
---
<span data-ttu-id="4a5f3-103">Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.</span><span class="sxs-lookup"><span data-stu-id="4a5f3-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="4a5f3-104">**Ключ на системния регистър**</span><span class="sxs-lookup"><span data-stu-id="4a5f3-104">**Registry key**</span></span>|<span data-ttu-id="4a5f3-105">Въведете</span><span class="sxs-lookup"><span data-stu-id="4a5f3-105">**Type**</span></span>|<span data-ttu-id="4a5f3-106">Стойност</span><span class="sxs-lookup"><span data-stu-id="4a5f3-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a5f3-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="4a5f3-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="4a5f3-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="4a5f3-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="4a5f3-109">1</span><span class="sxs-lookup"><span data-stu-id="4a5f3-109">1</span></span>  <br/> |
   
<span data-ttu-id="4a5f3-110">За повече информация вижте [Разрешаване модерни удостоверяване за офис 2013 на Windows устройства](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="4a5f3-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="4a5f3-p101">ЛОТАРИНГИЯ е активирана по подразбиране в Office 365 подпора и офис 2016. > отдалечен работен плот услуги (RDS) е предварително обявен за терминални услуги.</span><span class="sxs-lookup"><span data-stu-id="4a5f3-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

