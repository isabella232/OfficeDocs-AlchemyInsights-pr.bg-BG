---
title: Отстраняване на проблеми с гости
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939368"
---
# <a name="troubleshoot-guest-user-issues"></a>Отстраняване на проблеми с гости

1. За указания относно управлението на достъпа на гости до приложения вижте Управление [на достъпа на гости с рецензии за достъп на Azure AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Добавяне на гости към вашия справочник в портала на [Azure:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)В това бързо започване ще добавите нов потребител на гости към вашия справочник на Azure AD чрез портала на Azure, ще изпратите покана и ще видите как изглежда процесът на използване на поканата на потребителя.
1. [Добавяне на гост с PowerShell:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)В това бързо започване ще използвате командата New-AzureADMSInvitation, за да добавите един гост към вашия клиент на Azure.
1. За да научите как да присвоявате потребители и групи на корпоративни приложения в Azure Active Directory (Azure AD) или от портала на Azure, или с помощта на PowerShell, вижте Управление на възложната задача на потребител за приложение [в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. Azure Active Directory (Azure AD) B2B сътрудничеството работи с повечето приложения, които се интегрират с Azure AD. В тази [статия](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ще преминем през инструкции за конфигуриране на някои популярни приложения на SaaS за използване с Azure AD B2B.
1. Като организация, която използва възможности за сътрудничество Azure Active Directory (Azure AD) B2B, за да поканите гости от организации партньори към azure AD, сега можете да предоставите на тези потребители на B2B достъп до локалните приложения. Тези локални приложения могат да използват удостоверяване, базирано на SAML, или интегрирано Windows удостоверяване (IWA) с делегиране, ограничавано от Kerberos (KCD). За повече информация вижте [Предоставяне на B2B потребители в Azure AD достъп до вашите локални приложения.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Научете как да [дадете достъп на акаунтите на партньори,](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)управлявани от местно ниво, до ресурсите в облака чрез сътрудничество с Azure AD B2B.