---
title: 'Скенер на ПДИ: инсталиране и конфигуриране'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686631"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="33b91-102">Скенер на ПДИ: инсталиране и конфигуриране</span><span class="sxs-lookup"><span data-stu-id="33b91-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="33b91-103">**За да инсталирате скенера на ПДИ, следвайте препоръчваните указания**:</span><span class="sxs-lookup"><span data-stu-id="33b91-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="33b91-104">Ако надстройвате и не извършвате инсталация на чисто, моля, уверете се, че сте следвали насоките за [надстройване на програмата за защита на данните на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) и за унифициран клиент за етикетиране вижте [надстройване на инструмента за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="33b91-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="33b91-105">Проверете дали спазвате всички изисквания за [настройките на защитната стена и мрежова инфраструктура](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="33b91-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="33b91-106">Уверете се, че [правилата ви са настроени](https://docs.microsoft.com/azure/information-protection/configure-policy) за автоматично етикетиране или имат етикет по подразбиране в правилата.</span><span class="sxs-lookup"><span data-stu-id="33b91-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="33b91-107">Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [типовете файлове, поддържани от клиента за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="33b91-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="33b91-108">Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: [Промяна на нивото на защита по подразбиране на файлове](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="33b91-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="33b91-109">Уверете се, че потребителският акаунт, конфигуриран за изпълнение на услугата Scanner, има разрешения за достъп до всички конфигурирани хранилища.</span><span class="sxs-lookup"><span data-stu-id="33b91-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="33b91-110">Ако все още имате проблеми, можете да експортирате регистрите на скенера и да ги добавите към своя билет за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="33b91-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="33b91-111">**Експортиране на регистрационни файлове на скенера за защита на информацията на Azure**</span><span class="sxs-lookup"><span data-stu-id="33b91-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="33b91-112">Придвижете се до%localappdata%\Microsoft\MSIP под потребителския контекст, в който се изпълнява услугата Scanner.</span><span class="sxs-lookup"><span data-stu-id="33b91-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="33b91-113">Архивирайте цялото съдържание под папката MSIP.</span><span class="sxs-lookup"><span data-stu-id="33b91-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="33b91-114">Запишете регистрационните файлове по ваш избор и ги прикачете към вашата заявка за обслужване.</span><span class="sxs-lookup"><span data-stu-id="33b91-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="33b91-115">Можете също да използвате [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="33b91-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="33b91-116">**За допълнителна информация вж**.:</span><span class="sxs-lookup"><span data-stu-id="33b91-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="33b91-117">Разполагане на скенера за защита на информацията на Azure за автоматично класифициране и защита на файлове</span><span class="sxs-lookup"><span data-stu-id="33b91-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="33b91-118">Указване и използване на параметъра на маркера за Set-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="33b91-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="33b91-119">Изпълнение на цикъл на откриване и преглед на отчети за скенера</span><span class="sxs-lookup"><span data-stu-id="33b91-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="33b91-120">Преглед на документацията за защита на информацията на Azure</span><span class="sxs-lookup"><span data-stu-id="33b91-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="33b91-121">Изисквания за информация за Azure Protection</span><span class="sxs-lookup"><span data-stu-id="33b91-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="33b91-122">Изтегляне на Azure за защита на информацията за клиента</span><span class="sxs-lookup"><span data-stu-id="33b91-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
