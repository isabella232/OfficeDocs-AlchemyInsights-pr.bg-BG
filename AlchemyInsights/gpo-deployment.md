---
title: Разполагане на GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427014"
---
# <a name="gpo-deployment"></a><span data-ttu-id="0130e-102">Разполагане на GPO</span><span class="sxs-lookup"><span data-stu-id="0130e-102">GPO Deployment</span></span>

<span data-ttu-id="0130e-103">Настройките за обектите на потребителя и компютъра в Azure Active Directory Domain Services (Azure AD DS) често се управляват чрез обекти на групови правила (GPOs).</span><span class="sxs-lookup"><span data-stu-id="0130e-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="0130e-104">Azure AD DS включва вградени GPOs за контейнерите на AADDC и AADDC компютри.</span><span class="sxs-lookup"><span data-stu-id="0130e-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="0130e-105">Можете да персонализирате тези вградени GPOs, за да конфигурирате груповите правила, ако е необходимо за вашата среда.</span><span class="sxs-lookup"><span data-stu-id="0130e-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="0130e-106">Членовете на групата на Azure AD DC администраторите имат привилегии за администриране на груповите правила във владение на Azure AD DS и могат също да създават потребителски GPOs и организационни единици.</span><span class="sxs-lookup"><span data-stu-id="0130e-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="0130e-107">За повече информация относно правилата на групата и как работи, вижте [общ преглед на груповите правила](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span><span class="sxs-lookup"><span data-stu-id="0130e-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="0130e-108">В хибридна среда груповите правила, конфигурирани в локална среда на AD DS, не се синхронизират с Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="0130e-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="0130e-109">За да дефинирате настройки за конфигурация за потребители или компютри в Azure AD DS, редактирайте един от GPOs по подразбиране или създайте GPO по избор.</span><span class="sxs-lookup"><span data-stu-id="0130e-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="0130e-110">Тази статия [управление на груповите правила](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) ви показва как да инсталирате инструменти за управление на групови правила, как Ton редактирате вградения GPOs и как да създадете потребителски GPOs.</span><span class="sxs-lookup"><span data-stu-id="0130e-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
