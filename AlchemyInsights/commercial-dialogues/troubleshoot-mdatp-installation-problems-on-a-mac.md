---
title: Отстраняване на проблеми с инсталирането на MDATP на Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743738"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="259f8-102">Отстраняване на проблеми с инсталирането на MDATP на Mac</span><span class="sxs-lookup"><span data-stu-id="259f8-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="259f8-103">Ако ръчно инсталиране е неуспешно, страницата с **Резюме** на съветника за инсталиране показва следната грешка:</span><span class="sxs-lookup"><span data-stu-id="259f8-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="259f8-104">"Възникна грешка по време на инсталирането.</span><span class="sxs-lookup"><span data-stu-id="259f8-104">"An error occurred during installation.</span></span> <span data-ttu-id="259f8-105">Инсталиращата програма е срещнала грешка, която е накарала инсталацията да е неуспешна.</span><span class="sxs-lookup"><span data-stu-id="259f8-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="259f8-106">Свържете се с производителя на софтуера за помощ. "</span><span class="sxs-lookup"><span data-stu-id="259f8-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="259f8-107">За разполагания на MDM страницата показва и обща грешка при инсталирането.</span><span class="sxs-lookup"><span data-stu-id="259f8-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="259f8-108">Въпреки че не показваме точни грешки на крайните потребители, ние поддържаме регистрационен файл с напредъка на инсталацията в **/Library/logs/Microsoft/mdatp/Install.log**.</span><span class="sxs-lookup"><span data-stu-id="259f8-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="259f8-109">Всяка сесия за инсталиране се добавя към този регистрационен файл.</span><span class="sxs-lookup"><span data-stu-id="259f8-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="259f8-110">За да изведете само последната сесия за инсталиране, използвайте `sed` .</span><span class="sxs-lookup"><span data-stu-id="259f8-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="259f8-111">За да научите повече, вижте [отстраняване на проблеми с инсталирането за Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="259f8-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
