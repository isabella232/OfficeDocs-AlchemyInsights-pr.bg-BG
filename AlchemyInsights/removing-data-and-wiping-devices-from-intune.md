---
title: Премахване на данни и избърсване на устройства от Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438912"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="1c732-102">Премахване на данни и избърсване на устройства от Intune</span><span class="sxs-lookup"><span data-stu-id="1c732-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="1c732-103">Устройството Retire и Device Wipe remote действия могат да бъдат използвани за премахване на фирмени данни, управлявани от Intune или за извършване на фабрично нулиране и връщане на устройството към неговите настройки по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="1c732-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="1c732-104">Влезте в Microsoft 365 Управление на устройства и отидете **на Устройства**  >  **Всички устройства**.</span><span class="sxs-lookup"><span data-stu-id="1c732-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="1c732-105">Изберете устройството, което искате да изтриете.</span><span class="sxs-lookup"><span data-stu-id="1c732-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="1c732-106">Изберете типа отдалечено изтриване, което искате да направите.</span><span class="sxs-lookup"><span data-stu-id="1c732-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="1c732-107">Оттеглят изтрива само организационна информация, докато пълните изтривания възстановяват устройството до фабричните му настройки.</span><span class="sxs-lookup"><span data-stu-id="1c732-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="1c732-108">Изберете **Да** за потвърждение.</span><span class="sxs-lookup"><span data-stu-id="1c732-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="1c732-109">Докато изтриването завърши, състоянието на действието на устройството се показва като Retire Чакане.</span><span class="sxs-lookup"><span data-stu-id="1c732-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="1c732-110">След като действието приключи, вече няма да виждате мобилното устройство в списъка с управлявани устройства.</span><span class="sxs-lookup"><span data-stu-id="1c732-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="1c732-111">**Забележка:** Данните на компанията не могат да бъдат премахнати от устройства, съединени към Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1c732-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="1c732-112">За пълни подробности за ефекта на действията Retire и Wipe, включително това, което се запазва и какво се изтрива, вижте [Премахване на устройства чрез изтриване, оттегляне или ръчно отблясъло на устройството](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="1c732-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="1c732-113">За да изтриете всички данни от macOS устройство, вижте [Изтриване на всички данни от macOS устройство](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="1c732-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>