---
title: 'ОИП: Политики, които не се държат според очакванията'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580754"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="f60b1-102">ОИП: Политики, които не се държат според очакванията</span><span class="sxs-lookup"><span data-stu-id="f60b1-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="f60b1-103">Защита на информацията за Azure: правила не се държи според очакванията, вижте следните указания за препоръчителни указания за различни проблеми с правилата:</span><span class="sxs-lookup"><span data-stu-id="f60b1-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="f60b1-104">Ако имате проблеми с визуални маркировки, моля, прегледайте [Когато се прилагат визуални маркировки.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="f60b1-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="f60b1-105">Ако имате проблеми с автоматичното етикетиране, прегледайте [Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какви типове чувствителна информация [търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="f60b1-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="f60b1-106">Ако имате проблеми със защитата native/Pfile, прегледайте [конфигурацията на API на файла](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="f60b1-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="f60b1-107">Проверете дали използвате обхват правила, които не са конфигурирани правилно: [как да конфигурирате правилата за защита на информация за конкретен потребител с помощта на правила с обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="f60b1-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="f60b1-108">Ако автоматичното етикетиране не работи за Outlook прикачване на етикетиран документ, проверете дали DRMEncryptProperty не е дефиниран както е описано тук: [IRM настройки на системния регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="f60b1-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="f60b1-109">Ако все още имате проблеми, събира Azure информация защита клиентски регистрационни файлове и приложете експортираните регистрационни файлове на този билет.</span><span class="sxs-lookup"><span data-stu-id="f60b1-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="f60b1-110">Отворете документ на Office или създайте нов имейл в Outlook.</span><span class="sxs-lookup"><span data-stu-id="f60b1-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="f60b1-111">Щракнете върху **Защита/Помощ за чувствителност**  >  **и обратна връзка**.</span><span class="sxs-lookup"><span data-stu-id="f60b1-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="f60b1-112">Щракнете върху **Експортиране на регистрационни файлове**.</span><span class="sxs-lookup"><span data-stu-id="f60b1-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="f60b1-113">Запишете регистрационните файлове на ваш избор на местоположение и ги прикачете към тази заявка за услуга.</span><span class="sxs-lookup"><span data-stu-id="f60b1-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="f60b1-114">Допълнителни ресурси:</span><span class="sxs-lookup"><span data-stu-id="f60b1-114">Additional resources:</span></span>

- [<span data-ttu-id="f60b1-115">Как да конфигурирате етикет за визуални маркировки за Azure информация за защита</span><span class="sxs-lookup"><span data-stu-id="f60b1-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="f60b1-116">Преглед на документацията за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="f60b1-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="f60b1-117">Използване на етикети за чувствителност в приложения на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="f60b1-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

