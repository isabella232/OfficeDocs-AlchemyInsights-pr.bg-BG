---
title: Инсталиране на офис на терминален сървър-неразрешено
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205398"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="533b2-102">Инсталиране на Office на терминален сървър</span><span class="sxs-lookup"><span data-stu-id="533b2-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="533b2-103">За разполагане на Office 365 ProPlus на Windows Server с помощта на услуги за отдалечен работен плот (RDS), преди наименувани терминални услуги:</span><span class="sxs-lookup"><span data-stu-id="533b2-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="533b2-104">Трябва да имате Office 365 план, който включва Office 365 ProPlus, като например Office 365 Enterprise Еi или Enterprise е+.</span><span class="sxs-lookup"><span data-stu-id="533b2-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="533b2-105">Office 365 бизнес и Office 365 бизнес Премиум планове не включват Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="533b2-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="533b2-106">Трябва да активирате [споделено активиране на компютъра](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="533b2-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="533b2-107">Ако искате да инсталирате Office 365 ProPlus на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране***, използвайте следните стъпки.</span><span class="sxs-lookup"><span data-stu-id="533b2-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="533b2-108">Можете също да изтеглите и стартирате [Microsoft поддръжка и възстановяване помощник](https://aka.ms/SaRA_OfficeSCA_M365Portal) за инсталиране на Office 365 ProPlus в режим на споделена компютърна активация.</span><span class="sxs-lookup"><span data-stu-id="533b2-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="533b2-109">Проверете какъв план на Office 365 имате.</span><span class="sxs-lookup"><span data-stu-id="533b2-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="533b2-110">Научете как</span><span class="sxs-lookup"><span data-stu-id="533b2-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="533b2-111">Ако е необходимо, превключете към друг план на Office 365.</span><span class="sxs-lookup"><span data-stu-id="533b2-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="533b2-112">Научете как</span><span class="sxs-lookup"><span data-stu-id="533b2-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="533b2-113">Ако Office вече е инсталиран на RDS сървъра, използващ други планове на Office 365, деинсталирайте го.</span><span class="sxs-lookup"><span data-stu-id="533b2-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="533b2-114">Например, като отидете в контролния панел \> деинсталиране на програма.</span><span class="sxs-lookup"><span data-stu-id="533b2-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="533b2-115">Деинсталиране с помощта на [Microsoft support и помощник за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се занимаваш с проблеми.</span><span class="sxs-lookup"><span data-stu-id="533b2-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="533b2-116">RDS сървър Влезте в центъра за администриране на Microsoft 365 с администраторски акаунт и [Инсталирайте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="533b2-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="533b2-117">След инсталирането на Office, ***не отваряйте или влезте в*** приложения на Office.</span><span class="sxs-lookup"><span data-stu-id="533b2-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="533b2-118">RDS сървър Активирайте активиране на споделен компютър чрез редактиране на системния регистър, като следвате тези стъпки:</span><span class="sxs-lookup"><span data-stu-id="533b2-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="533b2-119">Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете изпълнение.</span><span class="sxs-lookup"><span data-stu-id="533b2-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="533b2-120">В полето Отвори въведете **regedit**и след това изберете OK.</span><span class="sxs-lookup"><span data-stu-id="533b2-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="533b2-121">Изберете да, когато бъдете подканени да позволите на редактора на системния регистър да направи промени в устройството.</span><span class="sxs-lookup"><span data-stu-id="533b2-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="533b2-122">В редактора на системния регистър, добавете низова стойност на **Ssydsлицензиране** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \оффице\кликкторун\конфигуратион.</span><span class="sxs-lookup"><span data-stu-id="533b2-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="533b2-123">RDS сървър, ***влезте като краен потребител*** и [Проверете дали е активирано споделено активиране за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="533b2-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="533b2-124">За повече информация относно предпоставки, настройка на инструкции и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [разполагане на office 365 ProPlus с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="533b2-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="533b2-125">За да коригирате грешки, свързани с активирането на споделен компютър, вижте [отстраняване на проблеми при активиране на споделен компютър за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="533b2-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  