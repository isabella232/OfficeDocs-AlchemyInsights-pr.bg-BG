---
title: Инсталиране на офис на терминален сървър - нелицензиран
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508617"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="d9250-102">Инсталиране на Office на терминален сървър</span><span class="sxs-lookup"><span data-stu-id="d9250-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="d9250-103">За разполагане на приложения на Microsoft 365 за enterprise на сървър на Windows с помощта на услуги за отдалечен работен плот (RDS), по-рано наречени терминални услуги:</span><span class="sxs-lookup"><span data-stu-id="d9250-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="d9250-104">Трябва да имате абонамент за Microsoft 365, който включва приложения на Microsoft 365 за корпоративни организации, като например Office 365 Enterprise E3 или Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="d9250-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="d9250-105">Приложенията на Microsoft 365 за бизнеса и приложенията на Microsoft 365 за бизнес премиум планове не включват приложения на Microsoft 365 за предприятие.</span><span class="sxs-lookup"><span data-stu-id="d9250-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="d9250-106">Трябва да активирате [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d9250-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="d9250-107">Ако искате да инсталирате Приложения на Microsoft 365 за enterprise на RDS от центъра за администриране на Microsoft 365, който използва настройките по подразбиране за ***инсталиране,*** използвайте следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="d9250-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="d9250-108">Можете също да изтеглите и стартирате помощника за поддръжка на [Microsoft и възстановяване,](https://aka.ms/SaRA_OfficeSCA_M365Portal) за да инсталирате приложения на Microsoft 365 за корпоративни в режим на активиране на споделен компютър.</span><span class="sxs-lookup"><span data-stu-id="d9250-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="d9250-109">Проверете какво имате абонамент за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d9250-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="d9250-110">Научете как</span><span class="sxs-lookup"><span data-stu-id="d9250-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="d9250-111">Ако е необходимо, преминете към друг абонамент за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d9250-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="d9250-112">Научете как</span><span class="sxs-lookup"><span data-stu-id="d9250-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="d9250-113">Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти на Microsoft 365, деинсталирайте го.</span><span class="sxs-lookup"><span data-stu-id="d9250-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="d9250-114">Например, като отидете в контролния панел \> Деинсталиране на програма.</span><span class="sxs-lookup"><span data-stu-id="d9250-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="d9250-115">Деинсталирайте с помощта [на поддръжката на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако имате проблеми.</span><span class="sxs-lookup"><span data-stu-id="d9250-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="d9250-116">На RDS сървъра влезте в центъра за администриране на Microsoft 365 с администраторския си акаунт и [инсталирайте приложения на Microsoft 365 за корпоративни](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="d9250-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="d9250-117">След инсталирането на Office ***не се отваря или влиза в*** приложения на Office.</span><span class="sxs-lookup"><span data-stu-id="d9250-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="d9250-118">RDS сървър разрешаване на активирането на споделения компютър чрез редактиране на системния регистър, като изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d9250-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="d9250-119">Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете Изпълнение.</span><span class="sxs-lookup"><span data-stu-id="d9250-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="d9250-120">В полето Отвори въведете **regedit**и след това изберете OK.</span><span class="sxs-lookup"><span data-stu-id="d9250-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="d9250-121">Изберете Да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени в устройството ви.</span><span class="sxs-lookup"><span data-stu-id="d9250-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="d9250-122">В редактора на системния регистър добавете низова стойност **на SharedComputerLicensing** с настройка на 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="d9250-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="d9250-123">RDS сървър ***влезте като краен потребител*** и проверете дали е разрешено активиране на [споделения компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="d9250-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="d9250-124">За повече информация относно предпоставките, инструкциите за инсталиране и указанията за потребителски инсталации с помощта на инструмента за разполагане на Office вижте разполагане на [Приложения на Microsoft 365 за предприятието с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="d9250-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="d9250-125">За да отстраните грешки, свързани с активирането на споделения компютър, вижте [Отстраняване на проблеми със споделените активиране на компютъра за Приложения на Microsoft 365 за корпоративни](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="d9250-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  