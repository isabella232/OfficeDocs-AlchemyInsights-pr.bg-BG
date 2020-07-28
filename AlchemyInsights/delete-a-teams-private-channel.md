---
title: Изтриване на частен канал на Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438753"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="5a22f-102">Изтриване на частен канал на Teams</span><span class="sxs-lookup"><span data-stu-id="5a22f-102">Delete a Teams private channel</span></span>

<span data-ttu-id="5a22f-103">Microsoft е наясно с проблем изтриване на екипи частен канал, ако имате Правила за задържане на SharePoint за съответния сайт на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5a22f-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="5a22f-104">Microsoft работи върху корекция.</span><span class="sxs-lookup"><span data-stu-id="5a22f-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="5a22f-105">Междувременно можете да използвате следните методи за изтриване на частен канал.</span><span class="sxs-lookup"><span data-stu-id="5a22f-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="5a22f-106">**Изключване на екип/колекция от сайтове от правилата за задържане на Sharepoint.**</span><span class="sxs-lookup"><span data-stu-id="5a22f-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="5a22f-107">Отидете на портала за администриране на Office 365 и изберете **Покажи всички** в левия навигационен екран.</span><span class="sxs-lookup"><span data-stu-id="5a22f-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="5a22f-108">Под Центрове за **администриране**отидете на Политика за защита & **съответствие с**  >  **правилата за предотвратяване на загубата на данни**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="5a22f-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="5a22f-109">Проверете всички правила, които се прилагат за сайтове на Sharepoint и променете правилата, така че сайтът на Sharepoint за екипа, съдържащ частния канал не е включена в правилата за задържане.</span><span class="sxs-lookup"><span data-stu-id="5a22f-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="5a22f-110">Запазете правилата.</span><span class="sxs-lookup"><span data-stu-id="5a22f-110">Save the policy.</span></span>
    <span data-ttu-id="5a22f-111">Може да отнеме до 24 часа, за да влязат в сила настройките на правилата.</span><span class="sxs-lookup"><span data-stu-id="5a22f-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="5a22f-112">След като сайтът е изключен, можете да изтриете частния канал.</span><span class="sxs-lookup"><span data-stu-id="5a22f-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="5a22f-113">***Възможно е да*** можете да изтриете частния канал, като използвате Екипи на Microsoft на вашето устройство с Android.</span><span class="sxs-lookup"><span data-stu-id="5a22f-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="5a22f-114">За свързана информация на SharePoint вижте [не може да изтриете елементи в SharePoint Online или OneDrive за бизнес](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="5a22f-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>