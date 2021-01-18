---
title: Конфигуриране на прокси сървър на приложението
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884801"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="58032-102">Конфигуриране на прокси сървър на приложението</span><span class="sxs-lookup"><span data-stu-id="58032-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="58032-103">За да разберете как да конфигурирате приложение за прокси сървър за приложения в Azure AD, за да изложите вашите локални приложения в облака, вижте [как да конфигурирате приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="58032-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="58032-104">Еднократната идентификация (SSO) позволява на вашите потребители да имат достъп до приложение без удостоверяване повече от един час.</span><span class="sxs-lookup"><span data-stu-id="58032-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="58032-105">Позволява на единното удостоверяване да се появява в облака, срещу Azure Active Directory и позволява на услугата или съединителя да се представя за потребителя, за да извърши допълнителни предизвикателства за удостоверяване от приложението.</span><span class="sxs-lookup"><span data-stu-id="58032-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="58032-106">За да научите повече, вижте [как да конфигурирате еднократна идентификация в приложение за прокси сървър на приложение](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="58032-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="58032-107">Използвайте [тази статия](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) , за да отстраните често срещани проблеми при създаването на ново приложение за прокси сървър на приложения.</span><span class="sxs-lookup"><span data-stu-id="58032-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="58032-108">Ако имате проблем със създаването на обратно удостоверяване към вашето приложение, може да се наложи да [отстраните конфигурациите на делегиране на Kerberos с ограничени права за прокси сървър за приложения](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) или да следвате указания за [Конфигуриране на приложението с PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , за да отстраните проблема си.</span><span class="sxs-lookup"><span data-stu-id="58032-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
