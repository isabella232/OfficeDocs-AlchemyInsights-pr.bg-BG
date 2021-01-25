---
title: Съпоставяне на атрибутите на потребителите
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949649"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="29a25-102">Съпоставяне на атрибутите на потребителите</span><span class="sxs-lookup"><span data-stu-id="29a25-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="29a25-103">За да отстраните известни проблеми със съпоставянето на атрибута, вижте [съпоставяния на атрибути](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="29a25-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="29a25-104">Microsoft Azure Active Directory (AD) предоставя поддръжка за осигуряването на потребители за приложения на други разработчици, като например Salesforce, G Suite и други.</span><span class="sxs-lookup"><span data-stu-id="29a25-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="29a25-105">Ако разрешите осигуряването на потребителя за приложение за SaaS от друг разработчик, порталът на Azure управлява стойностите на атрибута си чрез нанасяне на атрибут.</span><span class="sxs-lookup"><span data-stu-id="29a25-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="29a25-106">За да научите как да персонализирате атрибутите по подразбиране, вижте [Персонализиране на атрибута за осигуряване на потребители – съпоставяния за SaaS приложения в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="29a25-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="29a25-107">За да научите повече за осигуряването на потребителите в SaaS App, вижте [Какво представлява автоматизираното приложение за SaaS потребители в AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="29a25-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="29a25-108">При персонализиране на атрибута за съпоставяне на потребителски провизии е възможно да откриете, че атрибутът, който искате да съпоставите, не се показва в списъка на атрибута източник.</span><span class="sxs-lookup"><span data-stu-id="29a25-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="29a25-109">[Свойството синхронизиране на атрибут от локален указател на Active Directory в AZURE ad за осигуряване на](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) статия за приложения ви показва как да добавите липсващия атрибут, като го синхронизирате от локалната си реклама в Azure ad.</span><span class="sxs-lookup"><span data-stu-id="29a25-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
