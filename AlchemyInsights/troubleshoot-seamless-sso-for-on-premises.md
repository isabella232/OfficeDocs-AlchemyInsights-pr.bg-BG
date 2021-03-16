---
title: Отстраняване на безпроблемно еднократна идентификация (SSO) за локален
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816073"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="5c631-102">Отстраняване на безпроблемно еднократна идентификация (SSO) за локален</span><span class="sxs-lookup"><span data-stu-id="5c631-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="5c631-103">За да разрешите безпроблемните проблеми с еднократната идентификация (SSO), изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="5c631-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="5c631-104">**Как да прехвърлите ключа за дешифриране на Kerberos на акаунта за AZUREADSSO на компютъра?**</span><span class="sxs-lookup"><span data-stu-id="5c631-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="5c631-105">Горещо ви препоръчваме да прехвърлите ключа за дешифриране на Kerberos поне на всеки 30 дни.</span><span class="sxs-lookup"><span data-stu-id="5c631-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="5c631-106">За да направите това ръчно, вижте [как да прехвърлите ключове за дешифриране на Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="5c631-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="5c631-107">**Конфигуриране на "безпроблемна SSO"**</span><span class="sxs-lookup"><span data-stu-id="5c631-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="5c631-108">За да разположите безпроблемно SSO, следвайте стъпките в [Azure Active Directory безшевни еднократна идентификация: бърз старт](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="5c631-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="5c631-109">**Консултативния**</span><span class="sxs-lookup"><span data-stu-id="5c631-109">**Advisory**</span></span>

- <span data-ttu-id="5c631-110">[Azure Active Directory безшевни еднократна идентификация: често задавани въпроси](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) – в тази статия ние често задавани въпроси за Azure Active Directory безпроблемно един Sign-On (безшевни SSO).</span><span class="sxs-lookup"><span data-stu-id="5c631-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="5c631-111">Продължете да проверявате за ново съдържание.</span><span class="sxs-lookup"><span data-stu-id="5c631-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="5c631-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) -тази статия предоставя информация за това как да създавате искания за функции или да задавате технически въпроси относно безпроблемен див.</span><span class="sxs-lookup"><span data-stu-id="5c631-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="5c631-113">**Отстраняване**</span><span class="sxs-lookup"><span data-stu-id="5c631-113">**Troubleshoot**</span></span>

<span data-ttu-id="5c631-114">[Отстраняване на неизправности в Azure Active Directory безшевни еднократна идентификация](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) -тази статия ви помага да намерите информация за отстраняване на неизправности за често срещани проблеми по отношение на Azure Active Directory (Azure ad) безшевни единични Sign-On (безшевни SSO).</span><span class="sxs-lookup"><span data-stu-id="5c631-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







