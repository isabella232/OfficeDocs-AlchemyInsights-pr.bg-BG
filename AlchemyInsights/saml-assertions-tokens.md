---
title: SAML твърдения (жетони)
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
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884862"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="49bfe-102">SAML твърдения (жетони)</span><span class="sxs-lookup"><span data-stu-id="49bfe-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="49bfe-103">Твърдения за коректура на езика на SAML</span><span class="sxs-lookup"><span data-stu-id="49bfe-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="49bfe-104">По подразбиране SAML маркери за Windows Communication Foundation (WCF), използвани във външните сценарии за защита, се издават маркери.</span><span class="sxs-lookup"><span data-stu-id="49bfe-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="49bfe-105">За повече информация вижте [SAML жетони и рекламации](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span><span class="sxs-lookup"><span data-stu-id="49bfe-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="49bfe-106">Платформата за самоличност на Microsoft излъчва няколко типа маркери за защита в обработката на всеки поток на удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="49bfe-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="49bfe-107">[Справка за претенции за SAML](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) описва формата, характеристиките за защита и съдържанието на SAML 2,0 жетони.</span><span class="sxs-lookup"><span data-stu-id="49bfe-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="49bfe-108">Следвайте указанията в конфигуриране на [Токена за цял живот в платформата за самоличност на Microsoft,](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) за да разберете как да конфигурирате маркери за живот.</span><span class="sxs-lookup"><span data-stu-id="49bfe-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="49bfe-109">Следвайте стъпките, описани в [тази статия](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) , за да разберете как да конфигурирате шифроване на маркери на AZURE ad SAML.</span><span class="sxs-lookup"><span data-stu-id="49bfe-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="49bfe-110">В Azure AD можете да настроите опции за подписване на сертификат и алгоритъм за подписване на сертификат.</span><span class="sxs-lookup"><span data-stu-id="49bfe-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="49bfe-111">За повече информация вижте [Разширени опции за подписване на сертификат в SAML маркер за приложения на Gallery в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="49bfe-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
