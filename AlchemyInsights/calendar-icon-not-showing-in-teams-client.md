---
title: Икона за календар, която не се показва в Teams клиента
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819942"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="a6d7f-102">Икона за календар, която не се показва в Teams клиента</span><span class="sxs-lookup"><span data-stu-id="a6d7f-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="a6d7f-103">Разделът „Календар“ в Teams изисква достъп до пощенската кутия на Exchange чрез Exchange Web Services.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="a6d7f-104">Пощенската кутия на Exchange може да бъде онлайн или локална.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="a6d7f-105">За онлайн потребители, които не виждат раздела „Календар“, уверете се, че те[имат лиценз за пощенска кутия на Exchange Online и пощенската кутия е разрешена](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="a6d7f-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="a6d7f-106">Ако потребителят има валидна пощенска кутия в Exchange Online, но все още не може да види раздела „Календар“, е възможно да се сблъскате с проблем в мрежата.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="a6d7f-107">Използвайте инструмента [Анализатор за отдалечено свързване на Microsoft](https://testconnectivity.microsoft.com/) и стартирайте **Тестовете за свързване на Microsoft Exchange Web Services** за засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="a6d7f-108">Накрая проверете приложенията за [Teams – правила за настройка на приложения](https://admin.teams.microsoft.com/policies/app-setup), за да се гарантира, че приложението за календар не е премахнато от правилата, приложени към потребителя (най-вероятно **глобален (по подразбиране за организацията)**.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="a6d7f-109">Ако вашите потребители са разположени локално, трябва да потвърдите, че конфигурацията на хибридните ви системи е здрава.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="a6d7f-110">Използвайте [Съветника за конфигуриране на хибридно разполагане](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) за отстраняване на неизправностите.</span><span class="sxs-lookup"><span data-stu-id="a6d7f-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="a6d7f-111">Обърнете внимание, че [Teams изисква Exchange 2016 CU3 или по-нова версия](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="a6d7f-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
