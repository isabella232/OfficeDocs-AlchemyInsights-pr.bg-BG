---
title: Отстраняване на неизправности при хибридно присъединяване към Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401896"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="571a7-102">Отстраняване на неизправности при хибридно присъединяване към Azure AD</span><span class="sxs-lookup"><span data-stu-id="571a7-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="571a7-103">Силно препоръчително Уверете се, че едно устройство има достъп до крайни точки за регистриране на устройства под системния акаунт с помощта на скрипта [за свързване чрез регистриране на тестови устройства.](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)</span><span class="sxs-lookup"><span data-stu-id="571a7-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="571a7-104">Ако настройвате регистрации на устройства за първи път, не забравяйте да прегледате I[ntroduction to device management in Azure Active Directory,](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) за да научите как да получавате устройства под контрола на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="571a7-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="571a7-105">Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, уверете се, че сте [конфигурирали Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и първо [сте](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) поставили лицензирането.</span><span class="sxs-lookup"><span data-stu-id="571a7-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="571a7-106">Уверете се, че сте упълномощени да извършвате операции в Azure AD и локалната AD.</span><span class="sxs-lookup"><span data-stu-id="571a7-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="571a7-107">Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства.</span><span class="sxs-lookup"><span data-stu-id="571a7-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="571a7-108">Освен това, ако настройвате автоматични регистрации във вашия локален Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).</span><span class="sxs-lookup"><span data-stu-id="571a7-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="571a7-109">За повече подробности относно разрешаването на [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) потенциални проблеми с хибридното съединение вижте Отстраняване на неизправности при хибридно присъединяване за настройване на хибридно присъединяване към Azure AD и управление на устройства с помощта на портала на Azure Ad, вижте Настройване на хибридни устройства, присъединени към Azure AD (локално присъединени [домейни),](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) и Управление на устройства [с помощта на портала на Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="571a7-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="571a7-110">За да разрешите често срещани проблеми с присъединяването към хибриден Azure Active Directory (AD), вижте [ЧЗВ за хибридно присъединяване към Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)</span><span class="sxs-lookup"><span data-stu-id="571a7-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
