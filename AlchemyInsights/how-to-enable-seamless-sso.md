---
title: Как се разрешава безпроблемно SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780516"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="5d721-102">Как се разрешава безпроблемно SSO</span><span class="sxs-lookup"><span data-stu-id="5d721-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="5d721-103">Разрешете безпроблемно SSO чрез [AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="5d721-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="5d721-104">Ако изпълнявате нова инсталация на Azure AD Connect, изберете [пътя за инсталиране по избор](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="5d721-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="5d721-105">На страницата за **влизане на потребителя** изберете опцията разрешаване на **еднократна идентификация** .</span><span class="sxs-lookup"><span data-stu-id="5d721-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="5d721-106">За да се уверите, че сте разрешили безпроблемно SSO правилно:</span><span class="sxs-lookup"><span data-stu-id="5d721-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="5d721-107">Влезте в центъра за [администриране на Azure Active Directory](https://aad.portal.azure.com) като глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="5d721-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="5d721-108">Изберете **Azure Active Directory** в левия екран.</span><span class="sxs-lookup"><span data-stu-id="5d721-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="5d721-109">Проверете дали е **разрешена**безпроблемната еднократна идентификация.</span><span class="sxs-lookup"><span data-stu-id="5d721-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="5d721-110">За да научите повече, вижте [автоматично използване на Azure Active Directory: "бърз старт](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)".</span><span class="sxs-lookup"><span data-stu-id="5d721-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  