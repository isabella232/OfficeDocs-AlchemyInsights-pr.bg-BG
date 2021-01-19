---
title: Отстраняване на проблеми с потребителя за гости
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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900833"
---
# <a name="troubleshoot-guest-user-issues"></a>Отстраняване на проблеми с потребителя за гости

1. За насоки за управление на достъпа на гости до приложенията вижте [управление на достъпа на гости чрез отзиви за достъп до AZURE ad](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).
1. Можете [да добавите гости към своя указател в портала на Azure](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): в този бърз старт ще добавите нов гост към директорията на Azure ad чрез портала на Azure, ще изпратите покана и ще видите как изглежда процесът за изкупуване на поканата на потребителя за гост.
1. [Добавяне на гост потребител с PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): в този бърз старт ще използвате командата New-AzureADMSInvitation, за да добавите един гост към своя клиент на Azure.
1. За да научите как да присвоявате потребители и групи към корпоративни приложения в Azure Active Directory (Azure AD), от портала на Azure или с помощта на PowerShell, вижте [управление на задачата на потребителя за приложение в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal). 
1. B2B сътрудничеството за Azure Active Directory (Azure AD) работи с повечето приложения, които се интегрират с Azure AD. В тази [статия](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)Минаваме през инструкции за конфигуриране на някои популярни приложения SaaS за използване с AZURE ad B2B.
1. Като организация, използваща възможностите за B2B сътрудничество в Azure Active Directory (Azure AD), за да поканите гости от партньорските организации към вашата Azure AD, сега можете да осигурите достъп на тези B2B потребители до локални приложения. Тези локални приложения могат да използват удостоверяване, базирано на SAML, или интегрирано удостоверяване на Windows (IWA) с ограничена делегация на Kerberos (KCD). За повече информация вижте [предоставяне на B2B потребители в AZURE ad Access към вашите локални приложения](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).
1. Научете как да [дадете достъп на акаунтите за местно управление на партньор до ресурси в облака с помощта на AZURE ad B2B сътрудничество](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).