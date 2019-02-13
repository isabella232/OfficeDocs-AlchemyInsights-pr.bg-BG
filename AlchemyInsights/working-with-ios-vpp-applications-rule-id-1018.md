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
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917485"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="358c6-102">Работа с iOS VPP приложения</span><span class="sxs-lookup"><span data-stu-id="358c6-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="358c6-103">Прочетете [как да управлявате iOS приложения, закупени чрез Том-покупка програма с Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) да научите повече за функциите, ограничения и стъпки, за да използвате на Apple Том пазаруване програма и подкрепа за него в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="358c6-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="358c6-104">**Общи въпроси:** "Възложих iOS VPP ап за моите потребители, но инсталирането е неуспешно."</span><span class="sxs-lookup"><span data-stu-id="358c6-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="358c6-p101">Това може да се случи, ако една VPP маркер се използва в множество доставчици за управление на мобилно устройство. VPP символи от Apple може да се използва само с един доставчик. Ако сте използвали VPP точка маркер с няколко доставчици, трябва да качите отново знак Intune.</span><span class="sxs-lookup"><span data-stu-id="358c6-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="358c6-p102">Инсталацията също може да се провали, ако общият брой на инсталации надвишава броя на лицензи. За да видите на използване на доклад за вашите лицензи, отидете на **Intune мобилен apps** \> страницата **ап лицензи** . За да научите как да се възстановят лицензи в употреба, виж [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="358c6-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

