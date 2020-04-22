---
title: Работа с iOS VPP приложения Правило ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719946"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="60865-102">Работа с iOS VPP приложения</span><span class="sxs-lookup"><span data-stu-id="60865-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="60865-103">Прочетете [Как да управлявате iOS приложения, закупени чрез програма за закупуване на том с Microsoft Intune,](https://docs.microsoft.com/intune/vpp-apps-ios) за да научите за функции, ограничения и стъпки, за да се възползват от програмата apple Том покупка и подкрепата за него в Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="60865-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="60865-104">**Често срещани въпроси:** "Присвоих iOS VPP приложение на моите потребители, но инсталирането не беше успешно."</span><span class="sxs-lookup"><span data-stu-id="60865-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="60865-105">Това може да се случи, ако един VPP маркер се използва в няколко доставчици на мобилни устройства за управление.</span><span class="sxs-lookup"><span data-stu-id="60865-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="60865-106">VPP маркери от Apple могат да се използват само с един доставчик.</span><span class="sxs-lookup"><span data-stu-id="60865-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="60865-107">Ако сте използвали VPP маркер с няколко доставчика, трябва да качите отново маркера intune.</span><span class="sxs-lookup"><span data-stu-id="60865-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="60865-108">Инсталацията може да се провали, ако общият брой инсталации надвишава броя на лицензите.</span><span class="sxs-lookup"><span data-stu-id="60865-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="60865-109">За да видите отчет за употребата на лицензите си, отидете на страницата лицензи за приложения за мобилни **приложения** \> **в Intune.**</span><span class="sxs-lookup"><span data-stu-id="60865-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="60865-110">За да научите как да си възобновете лицензива в употреба, вижте [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="60865-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
