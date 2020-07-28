---
title: Управление на автоматичните актуализации за приложенията на Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438754"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="0ac46-102">Управление на автоматичните актуализации за приложенията на Office</span><span class="sxs-lookup"><span data-stu-id="0ac46-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="0ac46-103">По подразбиране актуализациите за приложенията на Office се изтеглят автоматично и се прилагат във фонов режим без намеса на потребителя.</span><span class="sxs-lookup"><span data-stu-id="0ac46-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="0ac46-104">Обаче администраторите могат да контролират как актуализациите се прилагат с помощта на настройките за актуализиране на Office.</span><span class="sxs-lookup"><span data-stu-id="0ac46-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="0ac46-105">Актуализиране на настройките позволяват на администраторите да разрешават или забраняват автоматичните актуализации, да показват или скриват бутона **"Актуализирай сега"** в Office, да зададете срокове за актуализиране и други.</span><span class="sxs-lookup"><span data-stu-id="0ac46-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="0ac46-106">За подробна информация вижте:</span><span class="sxs-lookup"><span data-stu-id="0ac46-106">For detailed information, see:</span></span>

- [<span data-ttu-id="0ac46-107">Конфигуриране на настройките за актуализация за Office</span><span class="sxs-lookup"><span data-stu-id="0ac46-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="0ac46-108">Не е разрешено автоматично актуализиране на Office</span><span class="sxs-lookup"><span data-stu-id="0ac46-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="0ac46-109">Определяне на начина на актуализиране на Office след инсталирането му</span><span class="sxs-lookup"><span data-stu-id="0ac46-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="0ac46-110">За да прегледате съществуващите настройки за актуализации, приложени към клиентски компютър, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="0ac46-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="0ac46-111">Отворете редактора на системния регистър, като **отидете да**  >  **стартирате**  >  **regedit**.</span><span class="sxs-lookup"><span data-stu-id="0ac46-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="0ac46-112">Превключете на следното местоположение и прегледайте настройките за актуализиране на Office:</span><span class="sxs-lookup"><span data-stu-id="0ac46-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="0ac46-113">A.</span><span class="sxs-lookup"><span data-stu-id="0ac46-113">a.</span></span> <span data-ttu-id="0ac46-114">HKEY_LOCAL_MACHINE\СОФТУЕР\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="0ac46-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="0ac46-115">B.</span><span class="sxs-lookup"><span data-stu-id="0ac46-115">b.</span></span> <span data-ttu-id="0ac46-116">Щракнете върху "Изпълнение\Конфигуриране"</span><span class="sxs-lookup"><span data-stu-id="0ac46-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="0ac46-117">**Забележка:**  Ако ключът OfficeMgmtCOM е зададен, може да видите "Актуализации се **Office**управляват от вашия системен администратор" съобщение в  >  **Office акаунт**Office  >  **актуализации**.</span><span class="sxs-lookup"><span data-stu-id="0ac46-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="0ac46-118">За повече информация вижте [Управление на актуализации на Приложения на Microsoft 365 с Диспечер на конфигурационните данни на Microsoft за крайна точка](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="0ac46-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  