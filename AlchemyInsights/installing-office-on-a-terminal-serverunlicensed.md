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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763206"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="22da5-102">Инсталиране на Office на терминален сървър</span><span class="sxs-lookup"><span data-stu-id="22da5-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="22da5-103">За разполагане на Приложения на Microsoft 365 за предприятие на Windows Server с помощта на услуги за отдалечен работен плот (RDS), наричани преди терминални услуги:</span><span class="sxs-lookup"><span data-stu-id="22da5-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="22da5-104">Трябва да имате абонамент за Microsoft 365, който включва приложения на Microsoft 365 за предприятие, като например Office 365 Enterprise E3 или Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="22da5-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="22da5-105">Microsoft 365 приложения за бизнес и Приложения на Microsoft 365 за бизнес планове Premium не включват приложения на Microsoft 365 за предприятие.</span><span class="sxs-lookup"><span data-stu-id="22da5-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="22da5-106">Трябва да разрешите [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="22da5-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="22da5-107">Ако искате да инсталирате Приложения на Microsoft 365 за предприятие на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране,*** използвайте следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="22da5-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="22da5-108">Можете също да изтеглите и стартирате поддръжката на [Microsoft и помощника](https://aka.ms/SaRA_OfficeSCA_M365Portal) за възстановяване, за да инсталирате Приложения на Microsoft 365 за предприятие в режим на активиране на споделен компютър.</span><span class="sxs-lookup"><span data-stu-id="22da5-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="22da5-109">Проверете какво абонамент за Microsoft 365 имате.</span><span class="sxs-lookup"><span data-stu-id="22da5-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="22da5-110">Научете как</span><span class="sxs-lookup"><span data-stu-id="22da5-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="22da5-111">Ако е необходимо, преминете към друг абонамент за Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="22da5-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="22da5-112">Научете как</span><span class="sxs-lookup"><span data-stu-id="22da5-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="22da5-113">Ако Office вече е инсталиран на RDS сървъра, който използва други абонаменти за Microsoft 365, деинсталирайте го.</span><span class="sxs-lookup"><span data-stu-id="22da5-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="22da5-114">Например, като отидете на \> контролния панел деинсталиране на програма.</span><span class="sxs-lookup"><span data-stu-id="22da5-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="22da5-115">Деинсталирайте с помощта [на Поддръжка на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се сближат с проблеми.</span><span class="sxs-lookup"><span data-stu-id="22da5-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="22da5-116">На RDS сървъра влезте в центъра за администриране на Microsoft 365 с акаунта на администратора и [инсталирайте Приложения на Microsoft 365 за предприятие](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="22da5-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="22da5-117">След инсталирането на ***Office, не отваряйте или не влизайте в*** приложения на Office.</span><span class="sxs-lookup"><span data-stu-id="22da5-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="22da5-118">На RDS сървъра разрешете активиране на споделен компютър чрез редактиране на системния регистър, като изпълните следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="22da5-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="22da5-119">Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете Изпълнение.</span><span class="sxs-lookup"><span data-stu-id="22da5-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="22da5-120">В полето Отвори въведете **regedit**и след това изберете OK.</span><span class="sxs-lookup"><span data-stu-id="22da5-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="22da5-121">Изберете Да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени във вашето устройство.</span><span class="sxs-lookup"><span data-stu-id="22da5-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="22da5-122">В редактора на системния регистър добавете низ стойност на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\СОФТУЕР\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="22da5-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="22da5-123">На RDS сървъра ***влезте като краен потребител*** и проверете дали активирането на [споделения компютър е разрешено за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="22da5-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="22da5-124">За повече подробности относно предпоставки, инструкции за инсталиране и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [Разполагане на приложения на Microsoft 365 за предприятието чрез услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="22da5-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="22da5-125">За да отстраните грешки, свързани с активирането на споделен компютър, вижте [Отстраняване на проблеми с активирането на споделен компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="22da5-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  