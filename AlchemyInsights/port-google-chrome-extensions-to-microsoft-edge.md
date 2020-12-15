---
title: Порт на Google Chrome разширения за Microsoft Edge (хром)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676846"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="eaad5-102">Порт на Google Chrome разширения за Microsoft Edge (хром)</span><span class="sxs-lookup"><span data-stu-id="eaad5-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="eaad5-103">Лесно е да изнесете [разширения на Google Chrome към Microsoft Edge (хром)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span><span class="sxs-lookup"><span data-stu-id="eaad5-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="eaad5-104">В повечето случаи са необходими само минимални промени, за да се изпълнят тези разширения в Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="eaad5-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="eaad5-105">API за разширение и manifest ключове, поддържани от Google Chrome, са съвместими с код с Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="eaad5-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="eaad5-106">Обаче Microsoft Edge не поддържа API за разширение на Chrome. gcm, Chrome. Identity. getAccounts, Chrome. Identity. getAuthToken и Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="eaad5-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>