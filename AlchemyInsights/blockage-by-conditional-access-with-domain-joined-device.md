---
title: Блокиран съм от условен достъп с устройство, което е присъединен към домейн
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035234"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="60602-102">Блокиран съм от условен достъп с устройство, което е присъединен към домейн</span><span class="sxs-lookup"><span data-stu-id="60602-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="60602-103">**Силно Препоръчителни инструменти**</span><span class="sxs-lookup"><span data-stu-id="60602-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="60602-104">[Инструмент за отстраняване на неизправности при регистриране на устройства](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – инструментът, който помага за отстраняване на най-често срещаните проблеми при регистриране на устройства.</span><span class="sxs-lookup"><span data-stu-id="60602-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="60602-105">[Скрипт за свързване на регистрационни устройства](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – скриптът, който помага да се гарантира, че устройството има достъп до крайните точки за регистрация на устройства под системния акаунт.</span><span class="sxs-lookup"><span data-stu-id="60602-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="60602-106">[Скрипт за изчистване на AZURE ad устройство](https://github.com/mzmaili/AzureADDeviceCleanup) – скриптът, който ви позволява да търсите и управлявате изхабени устройства във вашата среда.</span><span class="sxs-lookup"><span data-stu-id="60602-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="60602-107">Ето някои често срещани причини за условния достъп може да е неуспешно устройство, което е присъединен към домейн (хибридна Azure AD).</span><span class="sxs-lookup"><span data-stu-id="60602-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="60602-108">Няма **AZURE ad PRT на устройството** – трябва да се уверите, че устройството има маркер за основна обновяване на Azure ad (Prt).</span><span class="sxs-lookup"><span data-stu-id="60602-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="60602-109">За повече информация за PRT вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="60602-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="60602-110">За да се уверите, че имате Azure AD PRT, можете да изпълните `dsregcmd/status` командата на устройството и да проверите дали "AzureAdPrt" е равно на "да".</span><span class="sxs-lookup"><span data-stu-id="60602-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="60602-111">Ако "AzureAdPrt" е "не", проверете следното:</span><span class="sxs-lookup"><span data-stu-id="60602-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="60602-112">**Дали имате външна среда с AD FS и че е недостъпна за домашните мрежи на вашите потребители**: в този случай се уверете, че крайните точки на "usernamemixed" са достъпни от екстранет.</span><span class="sxs-lookup"><span data-stu-id="60602-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="60602-113">Ако вашият AD FS е зад VPN мрежа, се уверете, че потребителите се свързват с VPN и повторно влизане в устройството.</span><span class="sxs-lookup"><span data-stu-id="60602-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="60602-114">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span><span class="sxs-lookup"><span data-stu-id="60602-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="60602-115">**Дали TPM на устройството е повреден и следователно не може да удостовери устройството**: Проверете "TPM. msc", за да видите дали състоянието на TPM е "Готово".</span><span class="sxs-lookup"><span data-stu-id="60602-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="60602-116">Ако не е, изпълнете `dsregcmd/leave` и позволете на устройството да се присъедини повторно към AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="60602-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="60602-117">След това опитайте отново.</span><span class="sxs-lookup"><span data-stu-id="60602-117">Then, try again.</span></span> <span data-ttu-id="60602-118">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="60602-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="60602-119">**Използвате доставчик на самоличност, който не поддържа WS-Trust протокол**.</span><span class="sxs-lookup"><span data-stu-id="60602-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="60602-120">Както е описано в нашите документи, хибридните Azure AD-Съединени устройства не могат да работят в този случай.</span><span class="sxs-lookup"><span data-stu-id="60602-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="60602-121">Моля, Работете със своя доставчик на самоличност за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="60602-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="60602-122">**Потребителите използват браузъра Chrome без акаунти за Windows 10** или разширение на Office, като браузърът **не използва автоматично ПВЕ в устройства, свързани с пад или хибриден пад**: това води до неуспех на всички базирани на устройства правила за достъп под условие, като се показва съобщение за грешка "нерегистрирано устройство".</span><span class="sxs-lookup"><span data-stu-id="60602-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="60602-123">За да използвате правилно браузъра Chrome, трябва да инсталирате "акаунти за Windows 10" или "разширение на Office за браузъра на потребителите" чрез SCCM или в "Настройки".</span><span class="sxs-lookup"><span data-stu-id="60602-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="60602-124">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span><span class="sxs-lookup"><span data-stu-id="60602-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="60602-125">Ако не е възможно отдалечено да натискате разширението, уведомете потребителите, за да инсталирате ръчно едно от горните разширения, за да получите достъп до приложения зад условния достъп, базиран на устройства.</span><span class="sxs-lookup"><span data-stu-id="60602-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="60602-126">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span><span class="sxs-lookup"><span data-stu-id="60602-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="60602-127">**Устройството е правилно хибридно AZURE ad, но по невнимание е изтрито или забранено, поради което е необходимо да се синхронизират промените в AZURE ad Connect или от портала на Azure**: Ако това се случи, обектът на устройството вече не се разпознава като напълно присъединен план, въпреки че състоянието на "AzureAdJoined" и "PRT" се показва като валидно за устройството.</span><span class="sxs-lookup"><span data-stu-id="60602-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="60602-128">За да коригирате този проблем, изпълнете `dsregcmd/leave` на засегнатите устройства и им Позволете да се присъединят към AZURE ad.</span><span class="sxs-lookup"><span data-stu-id="60602-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="60602-129">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span><span class="sxs-lookup"><span data-stu-id="60602-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="60602-130">Ако вашите устройства са в Windows 10, актуализация на 1809, чрез прокси сървър за VPN/Cloud и вижте проблеми с "AzureAdPrt" или всяко приложение с проблем с SSO (Outlook не се свързва към пощенската кутия, въпреки че сте имали PRT), уверете се, че имате тази кръпка [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) или април сборна актуализация на [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , за да предотвратите неуспехите на ПВЕ на тези машини.</span><span class="sxs-lookup"><span data-stu-id="60602-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















