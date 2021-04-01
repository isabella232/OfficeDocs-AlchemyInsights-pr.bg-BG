---
title: Задаване на Microsoft Edge като браузър по подразбиране на устройство, присъединено към домейн
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
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491333"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="09ccb-102">Задаване на Microsoft Edge като браузър по подразбиране на устройство, присъединено към домейн</span><span class="sxs-lookup"><span data-stu-id="09ccb-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="09ccb-103">Задаване на Microsoft Edge като браузър по подразбиране:</span><span class="sxs-lookup"><span data-stu-id="09ccb-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="09ccb-104">[Създайте конфигурационен файл на асоциациите](https://go.microsoft.com/fwlink/?linkid=2132437) по подразбиране и го съхранявайте локално или в мрежов дял.</span><span class="sxs-lookup"><span data-stu-id="09ccb-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="09ccb-105">Отворете редактора на групови правила и след това отидете **на** Административни шаблони за  >  **конфигуриране на компютъра Windows**  >  **Components**  >  **File Explorer**.</span><span class="sxs-lookup"><span data-stu-id="09ccb-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="09ccb-106">Изберете **Задаване на конфигурационен файл за асоциации по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="09ccb-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="09ccb-107">Изберете **Настройка на правилата** и след това изберете **Разрешено**.</span><span class="sxs-lookup"><span data-stu-id="09ccb-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="09ccb-108">Под **Опции** въведете местоположението на конфигурационния файл на асоциациите по подразбиране и след това **изберете OK**.</span><span class="sxs-lookup"><span data-stu-id="09ccb-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
