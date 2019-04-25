---
title: Работа с iOS VPP приложения правило ИД 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420473"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="d98f2-102">Работа с iOS VPP приложения</span><span class="sxs-lookup"><span data-stu-id="d98f2-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="d98f2-103">Прочетете [как да управлявате iOS приложения, закупени чрез Том-покупка програма с Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) да научите повече за функциите, ограничения и стъпки, за да използвате на Apple Том пазаруване програма и подкрепа за него в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d98f2-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="d98f2-104">**Общи въпроси:** "Възложих iOS VPP ап за моите потребители, но инсталирането е неуспешно."</span><span class="sxs-lookup"><span data-stu-id="d98f2-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="d98f2-105">Това може да се случи, ако една VPP маркер се използва в множество доставчици за управление на мобилно устройство.</span><span class="sxs-lookup"><span data-stu-id="d98f2-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="d98f2-106">VPP символи от Apple може да се използва само с един доставчик.</span><span class="sxs-lookup"><span data-stu-id="d98f2-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="d98f2-107">Ако сте използвали VPP точка маркер с няколко доставчици, трябва да качите отново знак Intune.</span><span class="sxs-lookup"><span data-stu-id="d98f2-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="d98f2-108">Инсталацията също може да се провали, ако общият брой на инсталации надвишава броя на лицензи.</span><span class="sxs-lookup"><span data-stu-id="d98f2-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="d98f2-109">За да видите на използване на доклад за вашите лицензи, отидете на **Intune мобилен apps** \> страницата **ап лицензи** .</span><span class="sxs-lookup"><span data-stu-id="d98f2-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="d98f2-110">За да научите как да се възстановят лицензи в употреба, виж [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="d98f2-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

