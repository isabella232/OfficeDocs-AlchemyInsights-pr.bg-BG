---
title: Задаване на Microsoft Edge като браузър по подразбиране на macOS устройство
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491328"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="71d1c-102">Задаване на Microsoft Edge като браузър по подразбиране на macOS устройство</span><span class="sxs-lookup"><span data-stu-id="71d1c-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="71d1c-103">Използвайте един от тези два метода, за да зададете Microsoft Edge като браузър по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="71d1c-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="71d1c-104">Метод 1: Флаш устройството с изображение на macOS, където Microsoft Edge вече е зададен като браузър по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="71d1c-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="71d1c-105">Метод 2: Задайте правилата defaultBrowserSettingEnabled, за да подканите потребителя да зададете Microsoft Edge като браузър по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="71d1c-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="71d1c-106">И двата метода позволяват на потребителя да промени браузъра по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="71d1c-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="71d1c-107">Поради тази причина ви препоръчваме да разположите правилата DefaultBrowserSettingEnabled дори ако сте използвали метод 1.</span><span class="sxs-lookup"><span data-stu-id="71d1c-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="71d1c-108">Ако потребител промени браузъра по подразбиране след разполагането на правилата, правилата подканва потребителя да зададете браузъра по подразбиране обратно на Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="71d1c-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
