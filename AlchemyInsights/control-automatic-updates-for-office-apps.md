---
title: Управление на автоматични актуализации за приложенията на Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747765"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="c2fc2-102">Управление на автоматични актуализации за приложенията на Office</span><span class="sxs-lookup"><span data-stu-id="c2fc2-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="c2fc2-103">По подразбиране актуализациите за приложенията на Office се изтеглят автоматично и се прилагат във фона без намесата на потребителя.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="c2fc2-104">Администраторите обаче могат да управляват как се прилагат актуализациите с помощта на настройките на Office Update.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="c2fc2-105">Настройки за актуализиране Позволяване на администраторите да разрешават или забраняват автоматични актуализации, да показват или скриват бутона **Актуализирай сега** в Office, да задават срокове за актуализиране и др.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="c2fc2-106">За по-подробна информация вижте:</span><span class="sxs-lookup"><span data-stu-id="c2fc2-106">For detailed information, see:</span></span>

- [<span data-ttu-id="c2fc2-107">Конфигуриране на настройките за актуализиране за Office</span><span class="sxs-lookup"><span data-stu-id="c2fc2-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="c2fc2-108">Автоматичното актуализиране за Office не е разрешено</span><span class="sxs-lookup"><span data-stu-id="c2fc2-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="c2fc2-109">Определяне как Office да се актуализира, след като е инсталиран</span><span class="sxs-lookup"><span data-stu-id="c2fc2-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="c2fc2-110">За да прегледате съществуващите настройки за актуализации, приложени към клиентска машина, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="c2fc2-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="c2fc2-111">Отворете редактора на системния регистър, като отидете на **Старт**  >  **Run**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="c2fc2-112">Преминете към следното местоположение и Прегледайте настройките за актуализиране на Office:</span><span class="sxs-lookup"><span data-stu-id="c2fc2-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="c2fc2-113">на.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-113">a.</span></span> <span data-ttu-id="c2fc2-114">HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="c2fc2-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="c2fc2-115">b.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-115">b.</span></span> <span data-ttu-id="c2fc2-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="c2fc2-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="c2fc2-117">**Забележка**  Ако клавишът OfficeMgmtCOM е зададен, може да видите съобщение "актуализациите се управляват от вашия системен администратор **" в**актуализации на Office  >  **акаунт**за Office  >  **Office Updates**.</span><span class="sxs-lookup"><span data-stu-id="c2fc2-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="c2fc2-118">За повече информация вижте [управление на актуализациите за приложенията на microsoft 365 чрез диспечера за конфигуриране на крайна точка на Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="c2fc2-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  