---
title: Миграция от ГЛП към MIP/унифицирани етикети в центъра за съответствие
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
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236309"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="17874-102">Миграция от ГЛП към MIP/унифицирани етикети в центъра за съответствие</span><span class="sxs-lookup"><span data-stu-id="17874-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="17874-103">За да мигрирате от AIP етикети към единни етикети в центъра за защита и съответствие, направете следното:</span><span class="sxs-lookup"><span data-stu-id="17874-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="17874-104">**Активиране на защита от портала на Azure**</span><span class="sxs-lookup"><span data-stu-id="17874-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="17874-105">Ако още не сте го направили, отворете нов прозорец на браузъра и [влезте в портала на Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="17874-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="17874-106">Навигирайте до острието **за защита на информацията в Azure.**</span><span class="sxs-lookup"><span data-stu-id="17874-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="17874-107">Например в менюто на концентратор щракнете върху **всички услуги** и започнете да въвеждате **информация** в полето филтър .</span><span class="sxs-lookup"><span data-stu-id="17874-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="17874-108">Изберете **Защита на информацията в Azure**.</span><span class="sxs-lookup"><span data-stu-id="17874-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="17874-109">Ако не сте осъществили достъп до острието за защита на информацията в Azure преди, вижте еднократно [допълнителни стъпки,](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) за да добавите този нож към портала.</span><span class="sxs-lookup"><span data-stu-id="17874-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="17874-110">За да отворите острието за защита на информацията в Azure, трябва да имате [или план за защита на информацията в Azure,](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) или план на Office 365, който включва управление на правата.</span><span class="sxs-lookup"><span data-stu-id="17874-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="17874-111">Ако имате един от тези абонаменти, но видите съобщение, че не може да бъде намерен валиден абонамент, [се свържете с поддръжката на Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или използвайте стандартните канали за поддръжка.</span><span class="sxs-lookup"><span data-stu-id="17874-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="17874-112">Намерете опциите **на менюто Управление** и изберете Активиране на **защитата**.</span><span class="sxs-lookup"><span data-stu-id="17874-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="17874-113">Щракнете върху **Активиране**, след което потвърдете действието си.</span><span class="sxs-lookup"><span data-stu-id="17874-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="17874-114">Когато активирането завърши, информационната лента показва **активирането завърши успешно**.</span><span class="sxs-lookup"><span data-stu-id="17874-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="17874-115">**Мигриране на етикети за защита на информацията на Azure в Центъра за съответствие на & на Office 365**</span><span class="sxs-lookup"><span data-stu-id="17874-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="17874-116">Уверете се, че сте влезли като потребител с разрешение за глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="17874-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="17874-117">Навигирайте до острието **за защита на информацията в Azure.**</span><span class="sxs-lookup"><span data-stu-id="17874-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="17874-118">От опцията **Управление на** менюто изберете **Унифицирано етикетиране**.</span><span class="sxs-lookup"><span data-stu-id="17874-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="17874-119">В защита на **информацията за Azure - унифицирани етикетиране** blade click **Активиране** и следвайте онлайн инструкциите.</span><span class="sxs-lookup"><span data-stu-id="17874-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="17874-120">**Забележка**: Проверете дали имате необходимите разрешения преди активиране на защитата & съответствие център миграция.</span><span class="sxs-lookup"><span data-stu-id="17874-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="17874-121">Вижте тези статии за повече информация:</span><span class="sxs-lookup"><span data-stu-id="17874-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="17874-122">Трябва ли да сте глобален администратор, за да конфигурирате защитата на информацията в Azure или да делегирам на други администратори?</span><span class="sxs-lookup"><span data-stu-id="17874-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="17874-123">Важна информация за административни роли след мигриране на центъра за & съответствие на защитата.</span><span class="sxs-lookup"><span data-stu-id="17874-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="17874-124">За повече информация относно мигрирането на унифициран етикет към центъра за защита и съответствие вижте [Мигриране](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)на етикети .</span><span class="sxs-lookup"><span data-stu-id="17874-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
