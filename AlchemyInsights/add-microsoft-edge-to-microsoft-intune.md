---
title: Добавяне на Microsoft Edge към Microsoft за настройване
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194452"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="4a442-102">Добавяне на Microsoft Edge към Microsoft за настройване</span><span class="sxs-lookup"><span data-stu-id="4a442-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="4a442-103">За да можете да разположите, конфигурирате, наблюдавате и защитавате Microsoft Edge за Windows 10, трябва първо да го добавите към Microsoft.</span><span class="sxs-lookup"><span data-stu-id="4a442-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="4a442-104">В "Настройки" се поддържат Microsoft Edge 77 и по-нови версии.</span><span class="sxs-lookup"><span data-stu-id="4a442-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="4a442-105">Настройването ще открива всички съществуващи инсталации на Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="4a442-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="4a442-106">Ако Microsoft Edge е инсталиран в потребителски контекст, инсталирането на системата ще замести инсталацията в потребителски контекст.</span><span class="sxs-lookup"><span data-stu-id="4a442-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="4a442-107">Ако Microsoft Edge е инсталиран в системен контекст, ще бъде отчетен Успехът при инсталирането.</span><span class="sxs-lookup"><span data-stu-id="4a442-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="4a442-108">Предварително инсталирани Microsoft Edge 77 и по-нови версии за всички канали в потребителски контекст ще бъдат заменени с Microsoft Edge, инсталиран в системата контекст.</span><span class="sxs-lookup"><span data-stu-id="4a442-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="4a442-109">**Предпоставка**</span><span class="sxs-lookup"><span data-stu-id="4a442-109">**Prerequisite**</span></span>

<span data-ttu-id="4a442-110">Версия на Windows 10 1709 или по-нови версии</span><span class="sxs-lookup"><span data-stu-id="4a442-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="4a442-111">**Стъпки за добавяне на ръб за настройване**</span><span class="sxs-lookup"><span data-stu-id="4a442-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="4a442-112">[Конфигуриране на приложението в настройки](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="4a442-113">[Конфигуриране на информацията за приложението](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="4a442-114">[Конфигуриране на настройките на приложението](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="4a442-115">[Изберете етикетите за обхват (незадължително)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="4a442-116">[Добавете приложението](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="4a442-117">За допълнителна помощ вижте [отстраняване на неизправности](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="4a442-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




