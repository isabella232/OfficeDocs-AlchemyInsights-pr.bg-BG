---
title: 'ПДИ: правилата не се оказват по очаквания начин'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663178"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="751b7-102">ПДИ: правилата не се оказват по очаквания начин</span><span class="sxs-lookup"><span data-stu-id="751b7-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="751b7-103">Защита на информацията за Azure: правилата не се очакват по очаквания начин, вижте следните Препоръчителни указания за различни проблеми с правилата:</span><span class="sxs-lookup"><span data-stu-id="751b7-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="751b7-104">Ако имате проблеми с визуалните маркировки, моля, прегледайте [Кога се прилагат визуални маркировки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="751b7-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="751b7-105">Ако имате проблеми с автоматичното етикетиране, прегледайте [как да конфигурирате условия за автоматична и Препоръчителна класификация за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и [за какво се търсят типовете чувствителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="751b7-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="751b7-106">Ако имате проблеми с Native/Pfile Protection, моля, прегледайте [конфигурацията на API на файла](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="751b7-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="751b7-107">Проверете дали използвате правила за обхват, които не са конфигурирани правилно: [как да конфигурирате Azure Policy Protection за определени потребители, като използвате правила за обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="751b7-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="751b7-108">Ако автоматичното етикетиране не работи за Outlook при прикачването на документ с етикети, уверете се, че DRMEncryptProperty не е дефиниран, както е описано тук: [Настройки за IRM регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="751b7-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="751b7-109">Ако все още имате проблеми, моля, съберете регистрите на клиентите на Azure за защита на информацията и прикачете експортираните регистрационни файлове към този билет.</span><span class="sxs-lookup"><span data-stu-id="751b7-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="751b7-110">Отворете документ на Office или създайте ново имейл съобщение в Outlook.</span><span class="sxs-lookup"><span data-stu-id="751b7-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="751b7-111">Щракнете **Protect/Sensitivity**върху  >  **помощ и обратна връзка**за защита/чувствителност.</span><span class="sxs-lookup"><span data-stu-id="751b7-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="751b7-112">Щракнете върху **експортиране на регистрационни файлове**.</span><span class="sxs-lookup"><span data-stu-id="751b7-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="751b7-113">Запишете регистрите по ваш избор на местоположение и ги прикачете към това искане за обслужване.</span><span class="sxs-lookup"><span data-stu-id="751b7-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="751b7-114">Допълнителни ресурси:</span><span class="sxs-lookup"><span data-stu-id="751b7-114">Additional resources:</span></span>

- [<span data-ttu-id="751b7-115">Как да конфигурирате етикет за визуалните маркировки за Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="751b7-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="751b7-116">Преглед на документацията за защита на информацията на Azure</span><span class="sxs-lookup"><span data-stu-id="751b7-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="751b7-117">Използване на етикети за чувствителност в приложенията на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="751b7-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

