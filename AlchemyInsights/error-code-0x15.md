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
ms.openlocfilehash: 4ef2943e5a529368fa2c614e4431cf180924fbb8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36526962"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="f460f-103">Грешка при активиране офис 2013 на услугите за отдалечен работен плот</span><span class="sxs-lookup"><span data-stu-id="f460f-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="f460f-104">Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.</span><span class="sxs-lookup"><span data-stu-id="f460f-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="f460f-105">**Ключ на системния регистър**</span><span class="sxs-lookup"><span data-stu-id="f460f-105">**Registry key**</span></span>|<span data-ttu-id="f460f-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="f460f-106">**Type**</span></span>|<span data-ttu-id="f460f-107">**Стойност**</span><span class="sxs-lookup"><span data-stu-id="f460f-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f460f-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="f460f-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="f460f-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="f460f-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="f460f-110">1</span><span class="sxs-lookup"><span data-stu-id="f460f-110">1</span></span>  <br/> |

<span data-ttu-id="f460f-111">За повече информация вижте [Разрешаване модерни удостоверяване за офис 2013 на Windows устройства](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="f460f-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="f460f-112">ЛОТАРИНГИЯ е активирана по подразбиране в Office 365 подпора и офис 2016.</span><span class="sxs-lookup"><span data-stu-id="f460f-112">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="f460f-113">Отдалечен работен плот услуги (RDS) е предварително обявен за терминални услуги.</span><span class="sxs-lookup"><span data-stu-id="f460f-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  