---
title: Премахване на услугата за фон за Microsoft Search в Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816072"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="8b4ef-102">Премахване на услугата за фон за Microsoft Search в Bing</span><span class="sxs-lookup"><span data-stu-id="8b4ef-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="8b4ef-103">За да премахнете услугата за фон за Microsoft Search в Bing, можете да изпробвате следните корективни мерки:</span><span class="sxs-lookup"><span data-stu-id="8b4ef-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="8b4ef-104">За да се върнете към първоначалните настройки на системата за търсене, направете следните неща:</span><span class="sxs-lookup"><span data-stu-id="8b4ef-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="8b4ef-105">на.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-105">a.</span></span> <span data-ttu-id="8b4ef-106">Превключване на превключвателя за **използване на Bing като [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) търсачка по подразбиране**.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="8b4ef-107">b.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-107">b.</span></span> <span data-ttu-id="8b4ef-108">[Отидете в центъра за администриране на Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) и изчистете настройката, която засяга всички потребители във вашата организация.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="8b4ef-109">За да премахнете услугата за фон от отделно устройство, направете следните задачи:</span><span class="sxs-lookup"><span data-stu-id="8b4ef-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="8b4ef-110">на.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-110">a.</span></span> <span data-ttu-id="8b4ef-111">Изберете **Control Panel > програми > програми и функции**.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="8b4ef-112">b.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-112">b.</span></span> <span data-ttu-id="8b4ef-113">Щракнете с десния бутон върху **Microsoft Search в Bing** под списъка с инсталирани програми, след което щракнете върху **деинсталирай**.</span><span class="sxs-lookup"><span data-stu-id="8b4ef-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="8b4ef-114">За да премахнете услугата за заден фон от множество устройства във вашата организация, влезте като администратор и изпълнете следната команда в скрипт:</span><span class="sxs-lookup"><span data-stu-id="8b4ef-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
