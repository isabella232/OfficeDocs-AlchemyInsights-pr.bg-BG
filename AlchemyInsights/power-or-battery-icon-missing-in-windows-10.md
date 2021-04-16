---
title: Иконата за захранване или за батерията не се показва в Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790537"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="26fe2-102">Иконата за захранване или за батерията не се показва в Windows 10</span><span class="sxs-lookup"><span data-stu-id="26fe2-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="26fe2-103">Ако вашето устройство с Windows 10 има батерия (напр. лаптоп или таблет, или компютър, свързан чрез USB към UPS), обикновено в лентата на задачите се показва икона на захранване/батерията близо до часовника, например:</span><span class="sxs-lookup"><span data-stu-id="26fe2-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Икона на батерията](media/battery-icon.png)

<span data-ttu-id="26fe2-105">Ако не виждате тази икона, тя може да е скрита:</span><span class="sxs-lookup"><span data-stu-id="26fe2-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="26fe2-106">Отидете на **[Настройки > Персонализиране > Лента на задачите](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="26fe2-107">В областта за уведомяване, щракнете върху **Избор кои икони да се показват в лентата на задачите**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="26fe2-108">След това намерете елемента **Захранване** в списъка и превключете настройката му на **Включено**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Показване на иконата за захранване в лентата на задачите](media/power-icon-on.png)

<span data-ttu-id="26fe2-110">**Отстраняване на неизправности**</span><span class="sxs-lookup"><span data-stu-id="26fe2-110">**Troubleshooting**</span></span>

<span data-ttu-id="26fe2-111">Ако сте следвали инструкциите по-горе и превключвателят на **Захранване** е в сиво или не се вижда, в полето за търсене в лентата на задачите въведете **диспечера на устройствата**, след което изберете **Диспечер на устройствата** в списъка с резултати.</span><span class="sxs-lookup"><span data-stu-id="26fe2-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="26fe2-112">Под **Батерия**, щракнете с десния бутон върху батерията за вашето устройство, щракнете върху **Забраняване** и върху **Да**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="26fe2-113">Изчакайте няколко секунди и след това щракнете с десния бутон върху батерията и върху **Разрешаване**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="26fe2-114">След това рестартирайте устройството си.</span><span class="sxs-lookup"><span data-stu-id="26fe2-114">Then restart your device.</span></span>

<span data-ttu-id="26fe2-115">Ако сте изпълнили горните инструкции, но иконата на батерията не се показва в лентата на задачите, в полето за търсене в лентата на задачите въведете **диспечера на задачите** и след това щракнете върху **Диспечер на задачите** в списъка с резултати.</span><span class="sxs-lookup"><span data-stu-id="26fe2-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="26fe2-116">В раздела **Процеси**, под **Име**, щракнете с десния бутон върху **Explorer** и след това върху **Рестартиране**.</span><span class="sxs-lookup"><span data-stu-id="26fe2-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
