---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388234"
---
<span data-ttu-id="5b144-103">Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.</span><span class="sxs-lookup"><span data-stu-id="5b144-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="5b144-104">**Ключ на системния регистър**</span><span class="sxs-lookup"><span data-stu-id="5b144-104">**Registry key**</span></span>|<span data-ttu-id="5b144-105">**Тип**</span><span class="sxs-lookup"><span data-stu-id="5b144-105">**Type**</span></span>|<span data-ttu-id="5b144-106">**Стойност**</span><span class="sxs-lookup"><span data-stu-id="5b144-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5b144-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="5b144-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="5b144-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="5b144-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="5b144-109">1</span><span class="sxs-lookup"><span data-stu-id="5b144-109">1</span></span>  <br/> |

<span data-ttu-id="5b144-110">За повече информация вижте [Разрешаване модерни удостоверяване за офис 2013 на Windows устройства](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="5b144-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="5b144-111">ЛОТАРИНГИЯ е активирана по подразбиране в Office 365 подпора и офис 2016.</span><span class="sxs-lookup"><span data-stu-id="5b144-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="5b144-112">> отдалечен работен плот услуги (RDS) е предварително обявен за терминални услуги.</span><span class="sxs-lookup"><span data-stu-id="5b144-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  