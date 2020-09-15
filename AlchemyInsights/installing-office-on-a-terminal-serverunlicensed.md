---
title: Инсталиране на Office на терминален сървър – нелицензиран
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663106"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="091c8-102">Инсталиране на Office на терминален сървър</span><span class="sxs-lookup"><span data-stu-id="091c8-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="091c8-103">За разполагане на приложения на Microsoft 365 за Enterprise на сървър с Windows с помощта на услуги за отдалечен работен плот (RDS), наричани преди терминални услуги:</span><span class="sxs-lookup"><span data-stu-id="091c8-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="091c8-104">Трябва да имате абонамент за Microsoft 365, включващ приложения на Microsoft 365 за Enterprise, като например Office 365 Enterprise E3 или Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="091c8-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="091c8-105">Приложенията Microsoft 365 за бизнеса и приложенията на Microsoft 365 за Business Premium не включват приложенията на Microsoft 365 за Enterprise.</span><span class="sxs-lookup"><span data-stu-id="091c8-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="091c8-106">Трябва да разрешите [активирането на споделен компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="091c8-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="091c8-107">Ако искате да инсталирате приложенията на Microsoft 365 за Enterprise на RDS от центъра за администриране на Microsoft 365, ***който използва настройките за инсталиране по подразбиране***, използвайте стъпките по-долу.</span><span class="sxs-lookup"><span data-stu-id="091c8-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="091c8-108">Можете също да изтеглите и стартирате [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , за да инсталирате приложенията на Microsoft 365 за Enterprise в режима на активиране на споделен компютър.</span><span class="sxs-lookup"><span data-stu-id="091c8-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="091c8-109">Проверете какво представлява абонаментът за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="091c8-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="091c8-110">Научете как</span><span class="sxs-lookup"><span data-stu-id="091c8-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="091c8-111">Ако е необходимо, преминете към друг абонамент за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="091c8-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="091c8-112">Научете как</span><span class="sxs-lookup"><span data-stu-id="091c8-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="091c8-113">Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти за Microsoft 365, деинсталирайте го.</span><span class="sxs-lookup"><span data-stu-id="091c8-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="091c8-114">Например, като отидете в контролния панел, \> Деинсталирайте програма.</span><span class="sxs-lookup"><span data-stu-id="091c8-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="091c8-115">Деинсталирайте с помощта на [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ако се сблъскате с проблеми.</span><span class="sxs-lookup"><span data-stu-id="091c8-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="091c8-116">На сървъра RDS Влезте в центъра за администриране на Microsoft 365 със своя акаунт на администратор и [Инсталирайте приложенията на Microsoft 365 за Enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="091c8-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="091c8-117">След като Office е инсталиран, ***не отваряйте или не влизайте в*** никакви приложения на Office.</span><span class="sxs-lookup"><span data-stu-id="091c8-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="091c8-118">На RDS Server разрешете активирането на споделен компютър, като редактирате системния регистър, като изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="091c8-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="091c8-119">Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете изпълни.</span><span class="sxs-lookup"><span data-stu-id="091c8-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="091c8-120">В полето Отвори въведете **regedit**и след това изберете OK.</span><span class="sxs-lookup"><span data-stu-id="091c8-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="091c8-121">Изберете да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени на вашето устройство.</span><span class="sxs-lookup"><span data-stu-id="091c8-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="091c8-122">В редактора на системния регистър Добавете стойност на низ на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="091c8-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="091c8-123">На сървъра RDS ***влезте като краен потребител*** и [се уверете, че активирането на споделен компютър е разрешено за приложенията на Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="091c8-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="091c8-124">За повече информация относно предварителните изисквания, инструкции за настройка и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [разполагане на приложения на Microsoft 365 за Enterprise чрез отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="091c8-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="091c8-125">За да коригирате грешки, свързани с активирането на споделен компютър, вижте [отстраняване на проблеми при активиране на споделен компютър за приложенията Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="091c8-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  