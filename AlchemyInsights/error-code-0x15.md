---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате съобщение за грешка по време на активирането на Office 2013 при разполагане на отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709176"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="ddbf3-103">Грешка при активиране на Office 2013 в отдалечени настолни услуги</span><span class="sxs-lookup"><span data-stu-id="ddbf3-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="ddbf3-104">Ако получавате съобщение за грешка по време на активирането на Office 2013 при разполагане на отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.</span><span class="sxs-lookup"><span data-stu-id="ddbf3-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="ddbf3-105">**Ключ от системния регистър**</span><span class="sxs-lookup"><span data-stu-id="ddbf3-105">**Registry key**</span></span>|<span data-ttu-id="ddbf3-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="ddbf3-106">**Type**</span></span>|<span data-ttu-id="ddbf3-107">**Стойност**</span><span class="sxs-lookup"><span data-stu-id="ddbf3-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ddbf3-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="ddbf3-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="ddbf3-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="ddbf3-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="ddbf3-110">1</span><span class="sxs-lookup"><span data-stu-id="ddbf3-110">1</span></span>  <br/> |

<span data-ttu-id="ddbf3-111">За повече информация вижте [Разрешаване на модерното удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="ddbf3-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="ddbf3-112">ADAL е разрешено по подразбиране в приложенията Microsoft 365 за Enterprise и Office 2016.</span><span class="sxs-lookup"><span data-stu-id="ddbf3-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="ddbf3-113">Отдалечените настолни услуги (RDS) бяха предварително наименувани терминални услуги.</span><span class="sxs-lookup"><span data-stu-id="ddbf3-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  