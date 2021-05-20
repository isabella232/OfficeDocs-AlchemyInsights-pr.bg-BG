---
title: Няма съобщение за намерени абонаменти в центъра за защита
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544097"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="351ed-102">Няма съобщение за намерени абонаменти в центъра за защита</span><span class="sxs-lookup"><span data-stu-id="351ed-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="351ed-103">Ако при достъп до Microsoft Defender Security Center получите съобщение "Няма намерени абонаменти", това означава, че Azure Active Directory (AAD), използван за влизане на потребителя в портала, няма лиценз за Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="351ed-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="351ed-104">Лицензите Windows E5 и Office E5 са отделни лицензи.</span><span class="sxs-lookup"><span data-stu-id="351ed-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="351ed-105">Отворете случай на поддръжка, ако лицензът е закупен, но не е осигурен за този екземпляр на AAD.</span><span class="sxs-lookup"><span data-stu-id="351ed-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="351ed-106">Или имате:</span><span class="sxs-lookup"><span data-stu-id="351ed-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="351ed-107">Възможен проблем с осигуряването на лицензи.</span><span class="sxs-lookup"><span data-stu-id="351ed-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="351ed-108">Неволно сте предоставяли лиценза на друг Microsoft AAD от този, използван за удостоверяване в услугата.</span><span class="sxs-lookup"><span data-stu-id="351ed-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>