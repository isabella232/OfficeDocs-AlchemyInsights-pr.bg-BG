---
title: Отстраняване на проблеми с присъединяването към Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404257"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="d9ae6-102">Отстраняване на проблеми с присъединяването към Azure AD</span><span class="sxs-lookup"><span data-stu-id="d9ae6-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="d9ae6-103">Ако настройвате регистрации на устройства за първи път, уверете се, че сте прегледали Въведение в управлението на [устройства в Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) което ще ви напътства как да вземете Устройствата под контрола в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="d9ae6-104">Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, ще трябва да [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) се уверите, че първо сте конфигурирали [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) и че лицензирането е на първо място.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="d9ae6-105">Уверете се, че сте упълномощени да извършвате операции в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="d9ae6-106">Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства.</span><span class="sxs-lookup"><span data-stu-id="d9ae6-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="d9ae6-107">За да направите внедряването на Azure AD присъединяване, вижте [Планиране на Azure AD Присъединяване](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span><span class="sxs-lookup"><span data-stu-id="d9ae6-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="d9ae6-108">За повече подробности относно разрешаването на често срещани проблеми с присъединяването към [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) вж. ЧЗВ за присъединяване към Azure Ad и за устройства с Windows 10 pro вижте Не може да се присъедините към компютър с Windows 10 Pro към Azure AD – трябва да [надстроите до – общност на Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="d9ae6-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
