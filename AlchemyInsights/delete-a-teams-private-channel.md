---
title: Изтриване на личен канал за Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730904"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="6f02f-102">Изтриване на личен канал за Teams</span><span class="sxs-lookup"><span data-stu-id="6f02f-102">Delete a Teams private channel</span></span>

<span data-ttu-id="6f02f-103">Microsoft е наясно с проблем, който изтрива екипен личен канал, ако имате разрешени правила за съхранение на SharePoint за основния сайт на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6f02f-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="6f02f-104">Microsoft работи по корекция.</span><span class="sxs-lookup"><span data-stu-id="6f02f-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="6f02f-105">Междувременно можете да използвате следните заобиколни решения, за да изтриете частния канал.</span><span class="sxs-lookup"><span data-stu-id="6f02f-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="6f02f-106">**Изключвате колекцията от екипи/сайтове от правилата за съхранение на SharePoint.**</span><span class="sxs-lookup"><span data-stu-id="6f02f-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="6f02f-107">Отидете в портала за администриране на Office 365 и изберете **Покажи всички** в левия навигационен екран.</span><span class="sxs-lookup"><span data-stu-id="6f02f-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="6f02f-108">Под **центрове за администриране**отидете на **защита &**  >  правилата за предотвратяване на загуба на**данни**за съответствие  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="6f02f-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="6f02f-109">Определете правилата, които се отнасят за сайтовете на SharePoint, и променете правилата, така че сайтът на SharePoint за екипа, съдържащ частния канал, да не е включен в правилата за съхранение.</span><span class="sxs-lookup"><span data-stu-id="6f02f-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="6f02f-110">Запазете правилата.</span><span class="sxs-lookup"><span data-stu-id="6f02f-110">Save the policy.</span></span>
    <span data-ttu-id="6f02f-111">Възможно е да са необходими до 24 часа, за да влязат в сила настройките за правилата.</span><span class="sxs-lookup"><span data-stu-id="6f02f-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="6f02f-112">След като сайтът бъде изключен, можете да изтриете частния канал.</span><span class="sxs-lookup"><span data-stu-id="6f02f-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="6f02f-113">***Възможно*** е да успеете да изтриете частния канал с помощта на Microsoft Teams на устройството ви с Android.</span><span class="sxs-lookup"><span data-stu-id="6f02f-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="6f02f-114">За свързана информация в SharePoint вижте [не можете да изтривате елементи в SharePoint Online или OneDrive за бизнеса](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span><span class="sxs-lookup"><span data-stu-id="6f02f-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>