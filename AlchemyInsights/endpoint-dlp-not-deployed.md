---
title: Крайна точка DLP не е разположена на устройството на потребителя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731276"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="2fabe-102">Крайна точка DLP не е разположена на устройството на потребителя</span><span class="sxs-lookup"><span data-stu-id="2fabe-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="2fabe-103">Ако настройката за защита от загуба на данни на крайна точка (DLP) не е приложена към устройството на потребителя, уверете се, че отговаряте на тези изисквания:</span><span class="sxs-lookup"><span data-stu-id="2fabe-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="2fabe-104">Windows 10 x64 компилация 1809 или по-нова версия е инсталирана на устройството.</span><span class="sxs-lookup"><span data-stu-id="2fabe-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="2fabe-105">Инсталирана е версия 4.18.2009.7 или по-нова версия на злонамерен софтуер.</span><span class="sxs-lookup"><span data-stu-id="2fabe-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="2fabe-106">Устройството е **едно от** следните:</span><span class="sxs-lookup"><span data-stu-id="2fabe-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="2fabe-107">Azure Active Directory (Azure AD) присъединен</span><span class="sxs-lookup"><span data-stu-id="2fabe-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="2fabe-108">Хибридно присъединяване на Azure AD</span><span class="sxs-lookup"><span data-stu-id="2fabe-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="2fabe-109">AAD регистрирано</span><span class="sxs-lookup"><span data-stu-id="2fabe-109">AAD registered</span></span>

- <span data-ttu-id="2fabe-110">За да наложите действия по правилата, се уверете, че браузърът Chromium Edge на Microsoft е инсталиран на устройството с крайна точка.</span><span class="sxs-lookup"><span data-stu-id="2fabe-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="2fabe-111">За допълнителни изисквания за разполагане на DLP за крайна точка вижте [Първи стъпки в предотвратяването на загубата на данни за крайна точка.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="2fabe-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>