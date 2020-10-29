---
title: Отстраняване на неизправности при Microsoft Defender за Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801432"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="dc516-102">Отстраняване на неизправности при Microsoft Defender за Office 365</span><span class="sxs-lookup"><span data-stu-id="dc516-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="dc516-103">Забелязвате ли закъснения при доставяне на съобщения?</span><span class="sxs-lookup"><span data-stu-id="dc516-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="dc516-104">Използвайте опцията за [динамично доставяне](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) във вашата политика за безопасни прикачени файлове на ATP.</span><span class="sxs-lookup"><span data-stu-id="dc516-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="dc516-105">Това ще помогне за избягване на закъснения на съобщения, докато защитавате получателите от злонамерени файлове.</span><span class="sxs-lookup"><span data-stu-id="dc516-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="dc516-106">Искате ли да съобщите за грешни позитиви или фалшиви негативи в Microsoft?</span><span class="sxs-lookup"><span data-stu-id="dc516-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="dc516-107">Използвайте тази [връзка](https://www.microsoft.com/wdsi/filesubmission/) , за да подадете файлове за анализ.</span><span class="sxs-lookup"><span data-stu-id="dc516-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="dc516-108">Знаете ли, че можете да разрешите защитата за безопасни връзки за вътрешните имейли, изпратени между получателите във вашата организация?</span><span class="sxs-lookup"><span data-stu-id="dc516-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="dc516-109">Изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="dc516-109">Follow these steps:</span></span>

  1. <span data-ttu-id="dc516-110">Отидете на [https://protection.office.com](https://protection.office.com) и влезте с акаунт на глобален администратор или администратор на защитата.</span><span class="sxs-lookup"><span data-stu-id="dc516-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="dc516-111">В левия навигационния екран под **управление на заплахи** изберете **Policy** \> **връзки към безопасни** правила.</span><span class="sxs-lookup"><span data-stu-id="dc516-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="dc516-112">В раздела **правила, които важат за цялата организация** , изберете правилата и щракнете върху **Редактиране** .</span><span class="sxs-lookup"><span data-stu-id="dc516-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="dc516-113">Под **Настройки** разрешете **Приложете безопасни връзки към съобщенията, изпращани в рамките на организацията** .</span><span class="sxs-lookup"><span data-stu-id="dc516-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
