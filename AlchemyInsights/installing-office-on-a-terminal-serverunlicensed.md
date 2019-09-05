---
title: Инсталиране на офис на терминален сървър-неразрешено
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735378"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="db707-102">Инсталиране на Office на терминален сървър</span><span class="sxs-lookup"><span data-stu-id="db707-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="db707-103">За разполагане на Office 365 ProPlus на Windows Server с помощта на услуги за отдалечен работен плот (RDS), преди наименувани терминални услуги:</span><span class="sxs-lookup"><span data-stu-id="db707-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="db707-104">Трябва да имате Office 365 план, който включва Office 365 ProPlus, като например Office 365 Enterprise Еi или Enterprise е+.</span><span class="sxs-lookup"><span data-stu-id="db707-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="db707-105">Office 365 бизнес и Office 365 бизнес Премиум планове не включват Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="db707-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="db707-106">Трябва да активирате [споделено активиране на компютъра](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="db707-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="db707-107">Ако искате да инсталирате Office 365 ProPlus на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране***, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="db707-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="db707-108">Проверете какъв план на Office 365 имате.</span><span class="sxs-lookup"><span data-stu-id="db707-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="db707-109">Научете как</span><span class="sxs-lookup"><span data-stu-id="db707-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="db707-110">Ако е необходимо, превключете към друг план на Office 365.</span><span class="sxs-lookup"><span data-stu-id="db707-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="db707-111">Научете как</span><span class="sxs-lookup"><span data-stu-id="db707-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="db707-112">Ако Office вече е инсталиран на RDS сървъра, използващ други планове на Office 365, деинсталирайте го.</span><span class="sxs-lookup"><span data-stu-id="db707-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="db707-113">Например, като отидете в контролния панел \> деинсталиране на програма.</span><span class="sxs-lookup"><span data-stu-id="db707-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="db707-114">Деинсталиране с помощта на [Microsoft support и помощник за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се занимаваш с проблеми.</span><span class="sxs-lookup"><span data-stu-id="db707-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="db707-115">RDS сървър Влезте в центъра за администриране на Microsoft 365 с администраторски акаунт и [Инсталирайте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="db707-115">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="db707-116">След инсталирането на Office, ***не отваряйте или влезте в*** приложения на Office.</span><span class="sxs-lookup"><span data-stu-id="db707-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="db707-117">RDS сървър Активирайте активиране на споделен компютър чрез редактиране на системния регистър, като следвате тези стъпки:</span><span class="sxs-lookup"><span data-stu-id="db707-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="db707-118">Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете изпълнение.</span><span class="sxs-lookup"><span data-stu-id="db707-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="db707-119">В полето Отвори въведете **regedit**и след това изберете OK.</span><span class="sxs-lookup"><span data-stu-id="db707-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="db707-120">Изберете да, когато бъдете подканени да позволите на редактора на системния регистър да направи промени в устройството.</span><span class="sxs-lookup"><span data-stu-id="db707-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="db707-121">В редактора на системния регистър, добавете низова стойност на **Ssydsлицензиране** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \оффице\кликкторун\конфигуратион.</span><span class="sxs-lookup"><span data-stu-id="db707-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="db707-122">RDS сървър, ***влезте като краен потребител*** и [Проверете дали е активирано споделено активиране за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="db707-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="db707-123">За повече информация относно предпоставки, настройка на инструкции и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [разполагане на office 365 ProPlus с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="db707-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="db707-124">За да коригирате грешки, свързани с активирането на споделен компютър, вижте [отстраняване на проблеми при активиране на споделен компютър за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="db707-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  