---
title: Конфигуриране на LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884846"
---
# <a name="configure-ldap"></a><span data-ttu-id="d0b8b-102">Конфигуриране на LDAP</span><span class="sxs-lookup"><span data-stu-id="d0b8b-102">Configure LDAP</span></span>

<span data-ttu-id="d0b8b-103">За да конфигурирате LDAP, направете следното:</span><span class="sxs-lookup"><span data-stu-id="d0b8b-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="d0b8b-104">Проверете състоянието на вашия домейн в [портала на Azure](https://aka.ms/aadds-health).</span><span class="sxs-lookup"><span data-stu-id="d0b8b-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="d0b8b-105">Уверете се, че е наличен валиден абонамент за Azure AD, и услугите за домейни на Azure AD са разрешени.</span><span class="sxs-lookup"><span data-stu-id="d0b8b-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="d0b8b-106">Сертификатът, който е необходим за разрешаване на защитен LDAP, трябва да бъде получен от надежден публичен сертифициращ орган или да бъде самостоятелно подписан сертификат.</span><span class="sxs-lookup"><span data-stu-id="d0b8b-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="d0b8b-107">Проверете дали сертификатът следва необходимите [указания](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span><span class="sxs-lookup"><span data-stu-id="d0b8b-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="d0b8b-108">**Невалиден сертификат**</span><span class="sxs-lookup"><span data-stu-id="d0b8b-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="d0b8b-109">За да подновите сертификат, следвайте стъпките, за да създадете нов сертификат и повторно качване: [конфигурирайте LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d0b8b-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="d0b8b-110">За да отстраните известен проблем със защитени LDAP предупреждения в Azure Active Directory Domain Services, вижте [Разрешаване на LDAP известявания](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d0b8b-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>