---
title: Не е намерено съобщение "абонаменти" в центъра за защита
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713339"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="45900-102">Не е намерено съобщение "абонаменти" в центъра за защита</span><span class="sxs-lookup"><span data-stu-id="45900-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="45900-103">Ако при достъп до центъра за сигурност на Microsoft Defender получите съобщение "не са намерени абонаменти", това означава, че Azure Active Directory (пад), използван за влизане на потребителя в портала, няма лиценз за Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="45900-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="45900-104">Лицензите за Windows E5 и Office E5 са отделни лицензи.</span><span class="sxs-lookup"><span data-stu-id="45900-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="45900-105">Отворете калъф за поддръжка, ако лицензът е закупен, но не и осигурен за този екземпляр на пад.</span><span class="sxs-lookup"><span data-stu-id="45900-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="45900-106">Или имате:</span><span class="sxs-lookup"><span data-stu-id="45900-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="45900-107">Възможен проблем с осигуряването на лицензи.</span><span class="sxs-lookup"><span data-stu-id="45900-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="45900-108">По невнимание сте осигурили лиценза за различен Microsoft пад от този, който е използван за удостоверяване в услугата.</span><span class="sxs-lookup"><span data-stu-id="45900-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>