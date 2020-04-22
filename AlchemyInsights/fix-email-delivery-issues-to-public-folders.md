---
title: Отстраняване на проблеми с доставката на имейли до публични папки с разрешен за поща
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716341"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="bd4a6-102">Отстраняване на проблеми с доставката на имейли до публични папки с разрешен за поща</span><span class="sxs-lookup"><span data-stu-id="bd4a6-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="bd4a6-103">Ако външни податели не могат да изпращат съобщения до вашата поща разрешени публични папки и податели получават грешка: **не може да бъде намерен (550 5.4.1)**, проверете имейл домейн за публичната папка е конфигуриран като вътрешен препращане домейн вместо авторитетен домейн:</span><span class="sxs-lookup"><span data-stu-id="bd4a6-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="bd4a6-104">Отворете центъра за администриране на [Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="bd4a6-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="bd4a6-105">Отидете на **Пощенски поток** \> **Приети домейни**, изберете приетия домейн и след това щракнете върху **Редактиране**.</span><span class="sxs-lookup"><span data-stu-id="bd4a6-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="bd4a6-106">В страницата със свойства, която се отваря, ако типът домейн е зададен на **авторитетен**, променете стойността **на вътрешно реле** и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="bd4a6-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="bd4a6-107">Ако външни податели получите **грешка, нямате разрешение (550 5.7.13),** изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) да видите разрешенията за анонимни потребители в публичната папка:</span><span class="sxs-lookup"><span data-stu-id="bd4a6-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="bd4a6-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Например , `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="bd4a6-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="bd4a6-109">За да разрешите на външни потребители да изпращат имейл до тази публична папка, добавете правото createItems достъп до анонимен потребител.</span><span class="sxs-lookup"><span data-stu-id="bd4a6-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="bd4a6-110">Например , `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="bd4a6-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
