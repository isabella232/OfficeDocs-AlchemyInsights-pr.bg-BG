---
title: Етикетите за чувствителност не се показват
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801173"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="d9ee0-102">Етикетите за чувствителност не се показват</span><span class="sxs-lookup"><span data-stu-id="d9ee0-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="d9ee0-103">Етикетите за чувствителност ви позволяват да класифицирате и да защитавате чувствителното съдържание.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="d9ee0-104">Те могат да бъдат създадени в центъра за съответствие на Microsoft 365, в центъра за защита на Microsoft 365 или в центъра за защита на & на Microsoft 365 под класификация > етикети за чувствителност.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="d9ee0-105">За да научите повече за тази функция, вижте [общ преглед на етикетите за чувствителност](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="d9ee0-106">Ако сте конфигурирали вашите етикети за чувствителност, но те не се показват в приложенията на Microsoft 365, проверете следното:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="d9ee0-107">Уверете се, че етикетът за чувствителност е [публикуван](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) за потребителите и групите, които искате.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="d9ee0-108">Уверете се, че потребителят използва приложение, което поддържа етикети за чувствителност – вижте [етикети за чувствителност във вашия документ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="d9ee0-109">Ако [мигрирате етикети на Azure за защита на информацията](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), имайте предвид съображенията, описани [тук](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="d9ee0-110">Поддръжка за предотвратяване на загуба на данни (DLP): в момента само етикети за съхранение могат да бъдат използвани като условие в DLP правила.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="d9ee0-111">Поддръжката за етикети за чувствителност в DLP правилата все още не е налична, но работим по него.</span><span class="sxs-lookup"><span data-stu-id="d9ee0-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="d9ee0-112">Когато шифроването е разрешено на етикет за чувствителност, можете да изберете:</span><span class="sxs-lookup"><span data-stu-id="d9ee0-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="d9ee0-113">Присвояване на разрешения сега</span><span class="sxs-lookup"><span data-stu-id="d9ee0-113">Assign permissions now</span></span>
    - <span data-ttu-id="d9ee0-114">Позволяване на потребители да присвояват разрешения</span><span class="sxs-lookup"><span data-stu-id="d9ee0-114">Let users assign permissions</span></span>


<span data-ttu-id="d9ee0-115">За повече информация относно възможните проблеми вижте [известни проблеми с етикети за чувствителност](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="d9ee0-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>