---
title: Отстраняване на проблеми с доставянето на имейл до публични папки с активирана поща
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366453"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="c4e23-102">Отстраняване на проблеми с доставянето на имейл до публични папки с активирана поща</span><span class="sxs-lookup"><span data-stu-id="c4e23-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="c4e23-103">Ако външни податели не могат да изпращат съобщения до вашите публични папки с активиран имейл и подателите получат грешката: **не може да се намери (550 5.4.1)**, проверете дали домейнът за имейла за публичната папка е конфигуриран като вътрешен домейн за препращане, а не за достоверен домейн:</span><span class="sxs-lookup"><span data-stu-id="c4e23-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="c4e23-104">Отворете [центъра за администриране на Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="c4e23-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="c4e23-105">Отидете на **Mail flow** \> **приеманите домейни**"поща", изберете приетия домейн и след това щракнете върху **Редактиране**.</span><span class="sxs-lookup"><span data-stu-id="c4e23-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="c4e23-106">В страницата свойства, която се отваря, ако типът на домейна е зададен като **достоверен**, променете стойността на **вътрешно препращане** и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="c4e23-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="c4e23-107">Ако външни податели получат грешката, **която нямате разрешение (550 5.7.13)**, изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) , за да видите разрешенията за анонимни потребители в публичната папка:</span><span class="sxs-lookup"><span data-stu-id="c4e23-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="c4e23-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Например `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="c4e23-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="c4e23-109">За да разрешите на външни потребители да изпращат имейли до тази публична папка, добавете CreateItems Access направо към анонимния потребител.</span><span class="sxs-lookup"><span data-stu-id="c4e23-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="c4e23-110">Например `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="c4e23-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
