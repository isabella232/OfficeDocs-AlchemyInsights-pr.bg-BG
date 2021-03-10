---
title: Пример за Microsoft Defender за правилата за безопасни прикачени файлове на 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692584"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="bcde4-102">Пример за Microsoft Defender за правилата за безопасни прикачени файлове на 365</span><span class="sxs-lookup"><span data-stu-id="bcde4-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="bcde4-103">Тези настройки разрешават правила, за които *няма закъснения* , доставящи незабавно съобщения и след това прикачване на прикачени файлове след тяхното сканиране:</span><span class="sxs-lookup"><span data-stu-id="bcde4-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="bcde4-104">**Име**: няма закъснения</span><span class="sxs-lookup"><span data-stu-id="bcde4-104">**Name**: No delays</span></span>
- <span data-ttu-id="bcde4-105">**Описание**: доставя съобщения незабавно и повторно прикачване на прикачени файлове след сканиране.</span><span class="sxs-lookup"><span data-stu-id="bcde4-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="bcde4-106">**Отговор**: изберете опцията за **динамично доставяне** .</span><span class="sxs-lookup"><span data-stu-id="bcde4-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="bcde4-107">За повече информация вижте [динамични правила за доставяне в безопасни прикачени файлове](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="bcde4-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="bcde4-108">Секция за препращане на **прикачен файл** : изберете опцията, за да **разрешите пренасочване**, и след това въведете имейл адреса на своя глобален администратор на Microsoft 365, администратор на защитата или анализатор за защита, който ще разследва злонамерени прикачени файлове.</span><span class="sxs-lookup"><span data-stu-id="bcde4-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="bcde4-109">**Приложен към** раздел: изберете **домейна на получателя** и след това изберете своя домейн.</span><span class="sxs-lookup"><span data-stu-id="bcde4-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="bcde4-110">Изберете **Добави** и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="bcde4-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="bcde4-111">След като приключите, изберете **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="bcde4-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="bcde4-112">За да научите повече, вижте [безопасни прикачени файлове в Microsoft Defender за Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="bcde4-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
