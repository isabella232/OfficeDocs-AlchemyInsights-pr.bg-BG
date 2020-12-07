---
title: Поддръжката на Microsoft Edge за Microsoft Defender Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583250"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="906c5-102">Поддръжката на Microsoft Edge за Microsoft Defender Guard</span><span class="sxs-lookup"><span data-stu-id="906c5-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="906c5-103">Предназначена за Windows 10 и Microsoft Edge, Guard използва хардуерна изолация подход, който позволява на потребителя да навигира в ненадежден сайт от изолиран, Хипер-V контейнер, отделен от операционната система.</span><span class="sxs-lookup"><span data-stu-id="906c5-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="906c5-104">Корпоративен администратор определя списък с надеждни уеб сайтове, ресурси в облака и вътрешни мрежи.</span><span class="sxs-lookup"><span data-stu-id="906c5-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="906c5-105">Когато потребител посети сайт, който не е в списъка, Microsoft Edge ще отвори сайта в контейнера.</span><span class="sxs-lookup"><span data-stu-id="906c5-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="906c5-106">Това означава, че ако сайтът се окаже злонамерен, хост КОМПЮТЪРЪТ ще остане защитен и атакуващият няма да стигне до корпоративните данни.</span><span class="sxs-lookup"><span data-stu-id="906c5-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="906c5-107">Инсталирането на разширения в контейнера се поддържа като версия на Microsoft Edge 81 и може да се управлява чрез правилата.</span><span class="sxs-lookup"><span data-stu-id="906c5-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="906c5-108">Адресът на updateURL, който се използва в политиката на ExtensionInstallForcelist, трябва да бъде добавен като неутрален ресурс в правилата за изолация на мрежата, използвани от Guard за приложения.</span><span class="sxs-lookup"><span data-stu-id="906c5-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="906c5-109">За повече информация вижте [поддръжка на Microsoft Edge за Microsoft Defender Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span><span class="sxs-lookup"><span data-stu-id="906c5-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
