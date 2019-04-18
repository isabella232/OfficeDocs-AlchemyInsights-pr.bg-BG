---
title: Прикрепвам проблеми с имейл доставка с активирана поща публични папки
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910577"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="32437-102">Прикрепвам проблеми с имейл доставка с активирана поща публични папки</span><span class="sxs-lookup"><span data-stu-id="32437-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="32437-103">Ако външни податели не може да изпращате съобщения до вашите публични папки с активирана поща, и податели появи грешка: **не можа да се намери (550 5.4.1)**, проверка на имейл домейн за публичната папка е конфигуриран като домейн за вътрешно препредаване вместо достоверен домейн:</span><span class="sxs-lookup"><span data-stu-id="32437-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="32437-104">Отворете [центъра за администриране на Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="32437-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="32437-105">Отидете на **потока от поща** \> **приети домейни**, изберете приетият домейн и след това щракнете върху **Редактиране**.</span><span class="sxs-lookup"><span data-stu-id="32437-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="32437-106">В свойствата на страница това отваря, ако типът на домейна е зададен на **авторитетни**, променете стойността за **вътрешно препредаване** и след това щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="32437-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="32437-107">Ако външни податели грешка **нямате разрешение (550 5.7.13)**, изпълнете следната команда в [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) да видите разрешенията за анонимни потребители в публичната папка:</span><span class="sxs-lookup"><span data-stu-id="32437-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="32437-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`За пример `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="32437-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="32437-109">За да позволите на външни потребители да изпращат имейл до тази публична папка, добавете CreateItems достъп право на потребителя анонимен.</span><span class="sxs-lookup"><span data-stu-id="32437-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="32437-110">За пример `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="32437-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
