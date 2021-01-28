---
title: Проблеми с претенции за маркери и атрибути
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035833"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="9137c-102">Проблеми с претенции за маркери и атрибути</span><span class="sxs-lookup"><span data-stu-id="9137c-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="9137c-103">**Актуализиране, конфигуриране или премахване на претенции за маркери**</span><span class="sxs-lookup"><span data-stu-id="9137c-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="9137c-104">Чрез използването на Azure Active Directory (Azure AD) можете да [персонализирате типа на иск за иск за роля](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) в маркера за отговор, който получавате, след като упълномощите приложение.</span><span class="sxs-lookup"><span data-stu-id="9137c-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="9137c-105">Разработчиците на приложения могат да използват незадължителни искове в своите приложения на Azure AD, за да укажат кои претенции желаят в маркерите, изпратени до тяхното приложение.</span><span class="sxs-lookup"><span data-stu-id="9137c-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="9137c-106">За повече информация вижте [предоставяне на незадължителни искове за вашето приложение](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span><span class="sxs-lookup"><span data-stu-id="9137c-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="9137c-107">[Конфигуриране на групови искове за приложения с Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="9137c-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="9137c-108">Ако използвате безпроблемно еднократна идентификация във вашето приложение, вижте [Персонализиране на искове, издадени в SAML маркер за корпоративни приложения](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span><span class="sxs-lookup"><span data-stu-id="9137c-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="9137c-109">**Присвояване на атрибут за претенции**</span><span class="sxs-lookup"><span data-stu-id="9137c-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="9137c-110">За да конфигурирате правила за съпоставяне на искове с помощта на PowerShell, вижте [Персонализиране на искове, емитирани в маркери за конкретно приложение в клиент (предварителен преглед)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span><span class="sxs-lookup"><span data-stu-id="9137c-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="9137c-111">Атрибутите на справочното разширение на схемите предоставят начин да съхранявате допълнителни данни в Azure Active Directory в обекти на потребители и други обекти в указателя, като например групи, подробности за клиенти, основни услуги.</span><span class="sxs-lookup"><span data-stu-id="9137c-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="9137c-112">За емитиране на искове за приложения могат да се използват само атрибути за разширение на потребителските обекти.</span><span class="sxs-lookup"><span data-stu-id="9137c-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="9137c-113">[Използването на атрибути за разширение на схемата на справочен указател в искове](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) описва как да използвате атрибути за разширение на схеми на справочен указател за изпращане на потребителски данни към приложения в претенции за маркери.</span><span class="sxs-lookup"><span data-stu-id="9137c-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="9137c-114">За повече информация относно претенциите за маркери вижте:</span><span class="sxs-lookup"><span data-stu-id="9137c-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="9137c-115">Рекламации в маркерите на Access</span><span class="sxs-lookup"><span data-stu-id="9137c-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="9137c-116">Вземания в id_token</span><span class="sxs-lookup"><span data-stu-id="9137c-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="9137c-117">[Рекламации](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) , които можете да ОЧАКВАТЕ в ИД маркери и маркери за достъп, издадени от AZURE ad B2C</span><span class="sxs-lookup"><span data-stu-id="9137c-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="9137c-118">Справка за претенции за SAML</span><span class="sxs-lookup"><span data-stu-id="9137c-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
