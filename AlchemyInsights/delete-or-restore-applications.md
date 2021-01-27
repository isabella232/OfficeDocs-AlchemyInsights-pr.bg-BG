---
title: Изтриване или възстановяване на приложения
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014724"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="10506-102">Изтриване или възстановяване на приложения</span><span class="sxs-lookup"><span data-stu-id="10506-102">Delete or restore applications</span></span>

<span data-ttu-id="10506-103">**За да изтриете приложение от своя клиент на AZURE ad**:</span><span class="sxs-lookup"><span data-stu-id="10506-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="10506-104">В **портала на AZURE ad** изберете **корпоративни приложения**.</span><span class="sxs-lookup"><span data-stu-id="10506-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="10506-105">След това намерете и изберете приложението, което искате да изтриете.</span><span class="sxs-lookup"><span data-stu-id="10506-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="10506-106">В секцията **управление** в левия екран изберете **свойства**.</span><span class="sxs-lookup"><span data-stu-id="10506-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="10506-107">Изберете **Изтрий**, след което изберете **да** , за да потвърдите, че искате да изтриете приложението от вашия клиент на Azure ad.</span><span class="sxs-lookup"><span data-stu-id="10506-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="10506-108">За повече информация как да изтриете приложение, вижте бърз [Старт: Изтриване на приложение от клиент на Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="10506-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="10506-109">В PowerShell командата [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) премахва конфигурациите на прокси сървър за приложения от конкретно приложение в Azure Active Directory и може да изтрие напълно приложението, ако е зададено.</span><span class="sxs-lookup"><span data-stu-id="10506-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="10506-110">Можете да **възстановите изтрито приложение** с помощта на PowerShell.</span><span class="sxs-lookup"><span data-stu-id="10506-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="10506-111">След като приложението, което искате да възстановите, е идентифицирано, можете да го възстановите чрез [възстановяване на AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="10506-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
