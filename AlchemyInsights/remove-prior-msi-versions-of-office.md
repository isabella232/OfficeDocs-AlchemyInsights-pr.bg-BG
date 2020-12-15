---
title: Премахване на предишните версии на Office на MSI
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680651"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="a26aa-102">Премахване на предишните версии на Office на MSI</span><span class="sxs-lookup"><span data-stu-id="a26aa-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="a26aa-103">Препоръчвам премахване на предишна версия на Office на Windows Installer (MSI), преди да инсталирате Office 365 PROPLUS.</span><span class="sxs-lookup"><span data-stu-id="a26aa-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="a26aa-104">Ето как да направите това:</span><span class="sxs-lookup"><span data-stu-id="a26aa-104">Here's how to do this:</span></span>

1. <span data-ttu-id="a26aa-105">Ако сте използвали MSI за инсталиране на Office, можете да използвате инструмента за разполагане на Office (ODT), за да деинсталирате Office.</span><span class="sxs-lookup"><span data-stu-id="a26aa-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="a26aa-106">Можете да използвате елемента RemoveMSI във вашия **configuration.xml** файл.</span><span class="sxs-lookup"><span data-stu-id="a26aa-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="a26aa-107">Следвайте инструкциите в тази статия: [център за сигурност на & на Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="a26aa-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>