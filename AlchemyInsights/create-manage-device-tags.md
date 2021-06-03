---
title: Създаване и управление на етикети или групи на устройства
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731286"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="f0a0a-102">Създаване и управление на етикети или групи на устройства</span><span class="sxs-lookup"><span data-stu-id="f0a0a-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="f0a0a-103">Добавете етикети на устройства, за да създадете логическа принадлежност към група.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="f0a0a-104">Етикетите на устройства поддържат правилно съпоставяне на мрежата, което ви позволява да прикачвате различни етикети, за да заснемете контекста и да разрешите динамичното създаване на списъци като част от инцидент.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="f0a0a-105">Етикетите могат да се използват като филтър в списен изглед "Устройства" или за групиране на устройства.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="f0a0a-106">За повече информация относно групирането на устройства вижте [Създаване и управление на етикети на устройства](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="f0a0a-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="f0a0a-107">Можете да добавите етикети на устройства чрез:</span><span class="sxs-lookup"><span data-stu-id="f0a0a-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="f0a0a-108">Използване на портала</span><span class="sxs-lookup"><span data-stu-id="f0a0a-108">Using the portal</span></span>

- <span data-ttu-id="f0a0a-109">Задаване на стойност на ключ от системния регистър</span><span class="sxs-lookup"><span data-stu-id="f0a0a-109">Setting a registry key value</span></span>
 
<span data-ttu-id="f0a0a-110">**Забележка:** Възможно е да има закъснение между времето, когато етикетът се добавя към устройство и наличността му в списъка с устройства и страницата на устройството.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="f0a0a-111">За да добавите етикети на устройства с помощта на API, вижте [Добавяне или премахване на API за етикети на устройства](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="f0a0a-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="f0a0a-112">Добавяне и управление на етикети на устройства с помощта на портала</span><span class="sxs-lookup"><span data-stu-id="f0a0a-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="f0a0a-113">Изберете устройството, на което искате да управлявате етикетите.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="f0a0a-114">Можете да изберете или да потърсите устройство от някой от следните изгледи:</span><span class="sxs-lookup"><span data-stu-id="f0a0a-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="f0a0a-115">**Табло за операции за защита** Изберете името на устройството от раздела Най-добрите устройства с активни известия.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="f0a0a-116">**Опашка с предупреждения** – Изберете името на устройството до иконата на устройството от опашката с предупреждения.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="f0a0a-117">**Списък с устройства** – Изберете името на устройството от списъка с устройства.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="f0a0a-118">**Поле за** търсене – Изберете Устройство от падащото меню и въведете името на устройството.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="f0a0a-119">Можете също да стигнете до страницата за известяване чрез изгледите на файлове и IP адреси.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="f0a0a-120">Изберете **Управление на етикетите** от реда с действия за отговор.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="f0a0a-121">Въведете, за да намерите или създадете етикети.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-121">Type to find or create tags.</span></span>

<span data-ttu-id="f0a0a-122">Етикетите се добавят към изгледа на устройство и се отразяват в изгледа на списъка Устройства.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="f0a0a-123">След това можете да използвате филтъра етикети, за да видите съответния списък с устройства.</span><span class="sxs-lookup"><span data-stu-id="f0a0a-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="f0a0a-124">За повече информация вижте Създаване [и управление на етикети на устройства](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="f0a0a-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>