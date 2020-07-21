---
title: Потребителят получава грешка AADSTS7000112 Yammer е забранена
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197748"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="81531-102">Потребителят получава грешка AADSTS7000112 Yammer е забранена</span><span class="sxs-lookup"><span data-stu-id="81531-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="81531-103">Ако получите грешка "AADSTS7000112: приложение"00000005-0000-0ff1-ce00-000000000000000"(Yammer) е забранена", съществува проблем с принципал на услугата в Рамките на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="81531-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="81531-104">Администраторът може да е забранил принципа на услугата, за да блокира достъпа до Yammer.</span><span class="sxs-lookup"><span data-stu-id="81531-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="81531-105">Забраняването на принципа на услугата не се препоръчва и може да предизвика допълнителни проблеми.</span><span class="sxs-lookup"><span data-stu-id="81531-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="81531-106">За повече информация относно поддържания подход за блокиране на потребителски достъп до Yammer вижте [Изключване на достъпа на Yammer за потребители на Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="81531-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="81531-107">За да коригирате този проблем в Портала на Azure и възстановяване на потребителски достъп до Yammer:</span><span class="sxs-lookup"><span data-stu-id="81531-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="81531-108">Отворете страницата Azure Active Directory и изберете **Корпоративни приложения** в **управление** в левия навигационен екран.</span><span class="sxs-lookup"><span data-stu-id="81531-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="81531-109">Въведете **Office 365 Yammer** в полето за търсене и изберете името на приложението, за да отворите настройките.</span><span class="sxs-lookup"><span data-stu-id="81531-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="81531-110">Изберете **Свойства** под **Управление** в левия навигационен екран.</span><span class="sxs-lookup"><span data-stu-id="81531-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="81531-111">Задайте стойността на **разрешено за потребители да влизат в** **да**? След това изберете **Записване**.</span><span class="sxs-lookup"><span data-stu-id="81531-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="81531-112">Влезте отново в Yammer.</span><span class="sxs-lookup"><span data-stu-id="81531-112">Sign in to Yammer again.</span></span> <span data-ttu-id="81531-113">Може да се наложи да изчистите бисквитките.</span><span class="sxs-lookup"><span data-stu-id="81531-113">You might need to clear cookies.</span></span>

<span data-ttu-id="81531-114">Освен това изпълнете команди на PowerShell, за да зададете стойността.</span><span class="sxs-lookup"><span data-stu-id="81531-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="81531-115">За повече информация вижте ["Съжаляваме, но имаме проблеми с влизането ви в" грешка, когато щракнете върху плочката Yammer в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="81531-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 