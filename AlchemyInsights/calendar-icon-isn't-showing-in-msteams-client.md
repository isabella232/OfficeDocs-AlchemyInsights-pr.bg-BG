---
title: Иконата на календар не се показва в клиента на Microsoft Teams
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583200"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="b4a04-102">Иконата на календар не се показва в клиента на Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b4a04-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="b4a04-103">Разделът " **Календар** " в Teams изисква достъп до пощенската кутия на Exchange чрез уеб услугите на Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4a04-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="b4a04-104">Пощенската кутия на Exchange може да бъде онлайн или локална.</span><span class="sxs-lookup"><span data-stu-id="b4a04-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="b4a04-105">За онлайн потребители, които не виждат раздела **Календар** , се уверете, че [са лицензирани за пощенска кутия на Exchange Online и пощенската кутия е разрешена](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="b4a04-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="b4a04-106">Ако вашите потребители са домашно локални, трябва да потвърдите, че конфигурацията на вашия хибрид е здрава.</span><span class="sxs-lookup"><span data-stu-id="b4a04-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="b4a04-107">Използвайте [Съветника за конфигуриране на хибридно разполагане](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) за отстраняване на неизправностите.</span><span class="sxs-lookup"><span data-stu-id="b4a04-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="b4a04-108">Обърнете внимание, че [Teams изисква Exchange 2016 CU3 или по-нова версия](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="b4a04-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="b4a04-109">За повече информация и стъпки за отстраняване на неизправности вижте [отстраняване на проблеми с взаимодействието между Microsoft Teams и Exchange Server](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span><span class="sxs-lookup"><span data-stu-id="b4a04-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
