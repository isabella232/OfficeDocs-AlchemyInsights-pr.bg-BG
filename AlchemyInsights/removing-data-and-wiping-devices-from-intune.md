---
title: Премахване на данни и избърсване на устройства от "Настройки"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701272"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="f5ffe-102">Премахване на данни и избърсване на устройства от "Настройки"</span><span class="sxs-lookup"><span data-stu-id="f5ffe-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="f5ffe-103">Устройството се оттегля и избършете отдалечени действия могат да бъдат използвани за премахване на фирмените данни, управлявани чрез въвеждане или за извършване на нулиране на фабричните настройки и връщане на устройството към настройките по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="f5ffe-104">Влезте в Microsoft 365 за управление на устройства и отидете на **устройства**с  >  **всички устройства**.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="f5ffe-105">Изберете устройството, което искате да изтриете.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="f5ffe-106">Изберете типа отдалечено изтриване, което искате да направите.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="f5ffe-107">Оттегляне изтрива само организационна информация, докато пълните кърпички възстановяват устройството до фабричните му настройки.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="f5ffe-108">Изберете **да** , за да потвърдите.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="f5ffe-109">Докато избършете завърши, състоянието на действието на устройството се показва като изчакващо оттегляне.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="f5ffe-110">След като действието приключи, повече няма да виждате мобилното устройство в списъка с управлявани устройства.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="f5ffe-111">**Забележка** Фирмените данни не могат да бъдат премахнати от устройства, присъединени към Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f5ffe-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="f5ffe-112">За пълните подробности за ефекта на действията за оттегляне и избършете, включително какво се запазва и какво е изтрито, вижте [Премахване на устройства с помощта на изтриване, оттегляне или ръчно раззаписване на устройството](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="f5ffe-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="f5ffe-113">За изтриване на всички данни от устройство macOS вижте [Изтриване на всички данни от устройство с MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="f5ffe-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>