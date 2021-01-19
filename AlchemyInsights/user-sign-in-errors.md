---
title: Грешки при влизане в потребител
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900757"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="efd62-102">Грешки при влизане в потребител</span><span class="sxs-lookup"><span data-stu-id="efd62-102">User sign-in errors</span></span>

<span data-ttu-id="efd62-103">**Отстраняване на проблеми с диагностичната идентификация**</span><span class="sxs-lookup"><span data-stu-id="efd62-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="efd62-104">За откриване на проблемите с причината или диагностицирането, свързани с потребителското влизане, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="efd62-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="efd62-105">Стартирайте [диагностичната диагностика за влизане](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="efd62-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="efd62-106">Намерете събитието, което искате да анализирате чрез въвеждане на данните, които имате за потребителя, приложението, часа на влизане, ИД на заявка или ИД на корелация.</span><span class="sxs-lookup"><span data-stu-id="efd62-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="efd62-107">Прегледайте диагностичните резултати, които показват подробностите за това какво се е случило и какви действия можете да предприемете, за да направите промени, ако са необходими промени.</span><span class="sxs-lookup"><span data-stu-id="efd62-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="efd62-108">**Търсите информация за кодовете на грешки на AADSTS, върнати от услугата за маркери за защита на Azure Active Directory (Azure AD) (СТС)?**</span><span class="sxs-lookup"><span data-stu-id="efd62-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="efd62-109">Прочетете [тази статия](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , за да намерите описания на грешки в AADSTS, поправки и някои предложени заобиколни решения</span><span class="sxs-lookup"><span data-stu-id="efd62-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>