---
title: 'AIP: Правилата не се държат според очакванията'
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
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821616"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="de3da-102">AIP: Правилата не се държат според очакванията</span><span class="sxs-lookup"><span data-stu-id="de3da-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="de3da-103">Защита на информацията в Azure: Правилата не се държат според очакванията, вижте следното за препоръчителни указания за различни проблеми с правилата:</span><span class="sxs-lookup"><span data-stu-id="de3da-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="de3da-104">Ако имате проблеми с визуалните маркировки, прегледайте [При прилагане на визуални маркировки.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)</span><span class="sxs-lookup"><span data-stu-id="de3da-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="de3da-105">Ако имате проблеми с автоматичното етикетиране, прегледайте Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какво търси типовете [поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="de3da-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="de3da-106">Ако имате проблеми със защитата native/Pfile, прегледайте конфигурирането [на API на файл](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="de3da-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="de3da-107">Проверете дали използвате правила с обхват, които не са конфигурирани правилно: Как да конфигурирате правилата за защита на информацията в Azure за определени потребители с [помощта на правилата с обхват.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)</span><span class="sxs-lookup"><span data-stu-id="de3da-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="de3da-108">Ако автоматичното етикетиране не работи за Outlook, когато прикачвате етикетиран документ, проверете дали DRMEncryptProperty не е дефиниран по описания тук: Настройки на системния регистър [на IRM за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="de3da-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="de3da-109">Ако все още имате проблеми, съберете регистрационни файлове на клиента за защита на информацията в Azure и прикачете експортираните регистрационни файлове към този билет.</span><span class="sxs-lookup"><span data-stu-id="de3da-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="de3da-110">Отворете документ на Office или създайте нов имейл в Outlook.</span><span class="sxs-lookup"><span data-stu-id="de3da-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="de3da-111">Щракнете **върху Помощ за защита/чувствителност** и обратна  >  **връзка.**</span><span class="sxs-lookup"><span data-stu-id="de3da-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="de3da-112">Щракнете **върху Експортиране на регистрационни файлове**.</span><span class="sxs-lookup"><span data-stu-id="de3da-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="de3da-113">Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към тази заявка за услуга.</span><span class="sxs-lookup"><span data-stu-id="de3da-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="de3da-114">Допълнителни ресурси:</span><span class="sxs-lookup"><span data-stu-id="de3da-114">Additional resources:</span></span>

- [<span data-ttu-id="de3da-115">Как да конфигурирате етикет за визуални маркировки за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="de3da-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="de3da-116">Преглед на документацията за защита на информацията в Azure</span><span class="sxs-lookup"><span data-stu-id="de3da-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="de3da-117">Използване на етикети за чувствителност в приложения на Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="de3da-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

