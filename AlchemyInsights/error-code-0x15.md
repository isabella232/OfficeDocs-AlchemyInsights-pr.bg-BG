---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка при активиране на Office 2013 на услуги за отдалечен работен плот (RDS) разполагане, помислете за разрешаване на ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703127"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="ca4d4-103">Грешка при активиране на Office 2013 на услуги за отдалечен работен плот</span><span class="sxs-lookup"><span data-stu-id="ca4d4-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="ca4d4-104">Ако получавате грешка при активиране на Office 2013 на услуги за отдалечен работен плот (RDS) разполагане, помислете за разрешаване на ADAL чрез редактиране на системния регистър.</span><span class="sxs-lookup"><span data-stu-id="ca4d4-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="ca4d4-105">**Ключ на системния регистър**</span><span class="sxs-lookup"><span data-stu-id="ca4d4-105">**Registry key**</span></span>|<span data-ttu-id="ca4d4-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="ca4d4-106">**Type**</span></span>|<span data-ttu-id="ca4d4-107">**Стойност**</span><span class="sxs-lookup"><span data-stu-id="ca4d4-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ca4d4-108">HKEY_CURRENT_USER\Софтуер\Microsoft\Office\15.0\Общ\Самоличност\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="ca4d4-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="ca4d4-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ca4d4-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="ca4d4-110">1</span><span class="sxs-lookup"><span data-stu-id="ca4d4-110">1</span></span>  <br/> |

<span data-ttu-id="ca4d4-111">За повече информация вижте [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="ca4d4-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ca4d4-112">ADAL е разрешена по подразбиране в Microsoft 365 приложения за предприятие и Office 2016.</span><span class="sxs-lookup"><span data-stu-id="ca4d4-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="ca4d4-113">Услугите за отдалечен работен плот (RDS) вече са били наречени терминални услуги.</span><span class="sxs-lookup"><span data-stu-id="ca4d4-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  