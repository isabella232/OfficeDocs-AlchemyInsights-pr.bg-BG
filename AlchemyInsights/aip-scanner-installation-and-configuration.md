---
title: 'AIP скенер: инсталация и конфигурация'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357353"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="9f937-102">AIP скенер: инсталация и конфигурация</span><span class="sxs-lookup"><span data-stu-id="9f937-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="9f937-103">**За да инсталирате AIP скенера, следвайте препоръчителните указания:**</span><span class="sxs-lookup"><span data-stu-id="9f937-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="9f937-104">Ако надстройвате и не извършвате инсталация на чисто, уверете се, че сте следвали указанията за [надстройване на скенера](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) за защита на информацията на Azure и за обединен клиент за етикетиране, вижте [надстройване на скенера за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="9f937-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="9f937-105">Проверете дали отговаряте на [всички изисквания за настройките на защитната стена и мрежовата инфраструктура](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="9f937-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="9f937-106">Уверете се, че [правилата ви са зададени](https://docs.microsoft.com/azure/information-protection/configure-policy) на автоматично етикетиране или имат етикет по подразбиране в правилата.</span><span class="sxs-lookup"><span data-stu-id="9f937-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="9f937-107">Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [типове файлове, поддържани от клиента azure защита информация](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="9f937-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="9f937-108">Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: [Промяна на нивото на защита на файлове](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)по подразбиране .</span><span class="sxs-lookup"><span data-stu-id="9f937-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="9f937-109">Проверете дали потребителският акаунт е конфигуриран да изпълнява услугата на скенера, има разрешения за достъп до всички конфигурирани хранилища.</span><span class="sxs-lookup"><span data-stu-id="9f937-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="9f937-110">Ако все още имате проблеми, моля, експортирайте регистрационните файлове на скенера и ги добавете към вашия билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="9f937-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="9f937-111">**Експортиране на регистрационни файлове на скенера за защита на информация на Azure**</span><span class="sxs-lookup"><span data-stu-id="9f937-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="9f937-112">Навигирайте до %localappdata%\Microsoft\MSIP в контекста на потребителя, изпълняващ услугата на скенера.</span><span class="sxs-lookup"><span data-stu-id="9f937-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="9f937-113">Zip цялото съдържание в папката MSIP.</span><span class="sxs-lookup"><span data-stu-id="9f937-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="9f937-114">Запазете регистрационните файлове на вашия избор на местоположение и ги прикачете към заявката за услуги.</span><span class="sxs-lookup"><span data-stu-id="9f937-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="9f937-115">Можете също да използвате [експортиране-AIPLogs -OnuseOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="9f937-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="9f937-116">**За допълнителна информация вижте**:</span><span class="sxs-lookup"><span data-stu-id="9f937-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="9f937-117">Разполагане на скенера за защита на информация на Azure за автоматично класифициране и защита на файлове</span><span class="sxs-lookup"><span data-stu-id="9f937-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="9f937-118">Задайте и използвайте параметъра маркер за задаване aIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="9f937-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="9f937-119">Стартиране на цикъл на откриване и преглед на отчети за скенера</span><span class="sxs-lookup"><span data-stu-id="9f937-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="9f937-120">Преглед на документацията за защита на информация за Azure</span><span class="sxs-lookup"><span data-stu-id="9f937-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="9f937-121">Изисквания за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="9f937-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="9f937-122">Изтегляне на клиент абсбдис на информация за Azure</span><span class="sxs-lookup"><span data-stu-id="9f937-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
