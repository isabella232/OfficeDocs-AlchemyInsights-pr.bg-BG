---
title: Работа с ИД на правило за приложения на iOS с 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688935"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="8f955-102">Работа с приложения на iOS VPP</span><span class="sxs-lookup"><span data-stu-id="8f955-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="8f955-103">Прочетете [как да управлявате приложенията на IOS, закупени чрез програма за закупуване на обем, с Microsoft](https://docs.microsoft.com/intune/vpp-apps-ios) за да научите за функциите, ограниченията и стъпките, за да се възползвате от програмата за закупуване на томове на Apple и поддръжката за нея в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8f955-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="8f955-104">**Често срещани проблеми:** "Дадох на моите потребители приложение на iOS VPP, но инсталирането е неуспешно."</span><span class="sxs-lookup"><span data-stu-id="8f955-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="8f955-105">Това може да се случи, ако се използва единичен маркер за VPP точка в множество доставчици на управление на мобилни устройства.</span><span class="sxs-lookup"><span data-stu-id="8f955-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="8f955-106">VPP маркери от Apple могат да се използват само с един доставчик.</span><span class="sxs-lookup"><span data-stu-id="8f955-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="8f955-107">Ако сте използвали маркер на VPP точка с множество доставчици, трябва отново да качите маркера, за да го настроите.</span><span class="sxs-lookup"><span data-stu-id="8f955-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="8f955-108">Инсталацията може да се провали и ако общият брой на инсталациите надвишава броя на лицензите.</span><span class="sxs-lookup"><span data-stu-id="8f955-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="8f955-109">За да видите отчет за използването за вашите лицензи, отидете на страницата за лицензи за приложения на **мобилното** \> **приложение** .</span><span class="sxs-lookup"><span data-stu-id="8f955-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="8f955-110">За да научите как да поискате да се възстановят лицензи в употреба, вижте [тази статия.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="8f955-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
