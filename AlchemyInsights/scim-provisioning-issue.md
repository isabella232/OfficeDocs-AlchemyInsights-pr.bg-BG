---
title: Проблем с осигуряването на SCIM
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949653"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="1b0b3-102">Проблем с осигуряването на SCIM</span><span class="sxs-lookup"><span data-stu-id="1b0b3-102">SCIM provisioning issue</span></span>

<span data-ttu-id="1b0b3-103">Автоматизираното обезпечаване се отнася за създаването на потребителски самоличности и роли в приложенията в облака, до които потребителите имат нужда.</span><span class="sxs-lookup"><span data-stu-id="1b0b3-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="1b0b3-104">В допълнение към създаването на потребителски самоличности автоматичното осигуряване включва поддръжка и премахване на потребителските самоличности за промяна на състоянието или ролите.</span><span class="sxs-lookup"><span data-stu-id="1b0b3-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="1b0b3-105">Преди да започнете разполагане, можете да прегледате [как работи](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) осигуряването, за да научите как работи услугата Azure Active DIRECTORY (ad) и да получите препоръки за конфигуриране.</span><span class="sxs-lookup"><span data-stu-id="1b0b3-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="1b0b3-106">Като разработчик на приложения, можете да използвате системата за API за управление на самоличността между домейни (SCIM), за да разрешите автоматичното осигуряване на потребители и групи между вашата заявка и Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b0b3-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="1b0b3-107">[Крайна точка за създаване на SCIM и конфигуриране на осигуряването на потребителите с помощта на AZURE ad](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) описва как да създадете крайна точка на SCIM и да я интегрирате с услугата за осигуряване на Azure ad.</span><span class="sxs-lookup"><span data-stu-id="1b0b3-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



