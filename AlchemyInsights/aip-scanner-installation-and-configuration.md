---
title: 'AIP скенер: инсталиране и конфигуриране'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821652"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="7eb4d-102">AIP скенер: инсталиране и конфигуриране</span><span class="sxs-lookup"><span data-stu-id="7eb4d-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="7eb4d-103">**За да инсталирате AIP скенера, следвайте препоръчаните указания:**</span><span class="sxs-lookup"><span data-stu-id="7eb4d-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="7eb4d-104">Ако надстройвате и не извършвате чиста инсталация, уверете се, че сте следвали указанията за надстройване на [скенера за защита на информацията](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) на Azure и за унифициран клиент за етикети, вижте Надстройване на [скенера за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="7eb4d-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="7eb4d-105">Уверете се, че спазвате всички изисквания [за настройки на защитната стена и мрежовата инфраструктура.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="7eb4d-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="7eb4d-106">Уверете се, [че правилата ви са](https://docs.microsoft.com/azure/information-protection/configure-policy) зададени за автоматично етикети или имат етикет по подразбиране в правилата.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="7eb4d-107">Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [Типове файлове, поддържани от клиента за защита на информацията в Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="7eb4d-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="7eb4d-108">Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: Промяна на [нивото на защита по подразбиране на файловете.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="7eb4d-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="7eb4d-109">Уверете се, че потребителският акаунт, конфигуриран да изпълнява услугата за скенер, има разрешения за достъп до всички конфигурирани хранилища.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="7eb4d-110">Ако все още имате проблеми, експортирайте регистрационните файлове на скенера и ги добавете към билета си за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="7eb4d-111">**Експортиране на регистрационни файлове на скенера за защита на информацията в Azure**</span><span class="sxs-lookup"><span data-stu-id="7eb4d-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="7eb4d-112">Навигирайте до %localappdata%\Microsoft\MSIP под потребителския контекст, изпълняващ услугата за скенер.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="7eb4d-113">Zip цялото съдържание под папката MSIP.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="7eb4d-114">Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към вашата заявка за обслужване.</span><span class="sxs-lookup"><span data-stu-id="7eb4d-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="7eb4d-115">Можете също да използвате [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="7eb4d-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="7eb4d-116">**За допълнителна информация вижте**:</span><span class="sxs-lookup"><span data-stu-id="7eb4d-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="7eb4d-117">Разполагане на скенера за защита на информацията в Azure за автоматично класифициране и защита на файлове</span><span class="sxs-lookup"><span data-stu-id="7eb4d-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="7eb4d-118">Задаване и използване на параметъра "Маркер" за Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="7eb4d-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="7eb4d-119">Изпълнение на цикъл на откриване и преглед на отчети за скенера</span><span class="sxs-lookup"><span data-stu-id="7eb4d-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="7eb4d-120">Преглед на документацията за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="7eb4d-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7eb4d-121">Изисквания за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="7eb4d-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="7eb4d-122">Изтегляне на клиента за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="7eb4d-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
