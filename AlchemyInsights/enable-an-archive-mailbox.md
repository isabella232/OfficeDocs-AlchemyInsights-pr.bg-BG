---
title: Разрешаване на архивна пощенска кутия
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 3e20eaf8dec85454ce5a67e1b21292b2a33ebb1d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47811694"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="04c63-102">Разрешаване на архивна пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="04c63-102">Enable an archive mailbox</span></span>

<span data-ttu-id="04c63-103">Ако искате да изпълняваме автоматизирани проверки, за да гарантираме, че пощенската кутия за архивиране може да бъде конфигурирана, изберете бутона Назад <--в горния край на тази страница и след това въведете имейл адреса на акаунта.</span><span class="sxs-lookup"><span data-stu-id="04c63-103">If you want us to run automated checks to ensure an archive mailbox can be configured, select the back button <-- at the top of this page, and then enter the email address of the account.</span></span>

<span data-ttu-id="04c63-104">Архивирайте пощенските кутии в Microsoft 365 (наричани също *онлайн архиви* или *архиви на място*) Осигурете на потребителите допълнително място за съхранение на имейл.</span><span class="sxs-lookup"><span data-stu-id="04c63-104">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="04c63-105">Потребителите могат да преместват или копират елементи в своята архивна пощенска кутия и администраторите могат да създадат правила за архивиране, които автоматично преместват елементи за архивиране на пощенските кутии.</span><span class="sxs-lookup"><span data-stu-id="04c63-105">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="04c63-106">Ето как да създадете архивна пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="04c63-106">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="04c63-107">Отиване на [https://protection.office.com](https://protection.office.com) .</span><span class="sxs-lookup"><span data-stu-id="04c63-107">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="04c63-108">Влезте в Microsoft 365 чрез своя акаунт на администратор.</span><span class="sxs-lookup"><span data-stu-id="04c63-108">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="04c63-109">В левия екран на центъра за съответствие на защитата &amp; Изберете Архив за **управление на информацията** \> **Archive**.</span><span class="sxs-lookup"><span data-stu-id="04c63-109">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="04c63-110">Изберете потребителя, чиято архивна пощенска кутия искате да разрешите.</span><span class="sxs-lookup"><span data-stu-id="04c63-110">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="04c63-111">В екрана за подробни данни отдясно щракнете върху **Разреши** и след това щракнете върху **да** в предупредителното съобщение, за да разрешите архивната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="04c63-111">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="04c63-112">Можете също да разрешите групово архивиране на пощенските кутии, като изберете множество потребители (с помощта на клавишите **Shift** или **Ctrl** ) и след това щракнете върху **Разреши** в екрана за подробни данни.</span><span class="sxs-lookup"><span data-stu-id="04c63-112">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="04c63-113">Споделени пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="04c63-113">Shared mailboxes</span></span>

<span data-ttu-id="04c63-114">За да разрешите архивирането за споделена пощенска кутия, лиценз за план 2 за Exchange Online или лиценз на Exchange Online (план 1) с лиценз за архивиране на Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="04c63-114">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="04c63-115">За да разрешите архивирането за споделена пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="04c63-115">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="04c63-116">Отидете в [центъра за администриране на Exchange](https://outlook.office365.com/ecp) и влезте със своя акаунт на администратор.</span><span class="sxs-lookup"><span data-stu-id="04c63-116">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="04c63-117">Отидете на **Recipients**  >  **споделени**получатели.</span><span class="sxs-lookup"><span data-stu-id="04c63-117">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="04c63-118">Изберете споделената пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="04c63-118">Select the shared mailbox.</span></span>

4. <span data-ttu-id="04c63-119">В екрана за подробни данни отдясно, под **архивиране на места**щракнете върху **Разреши**и след това щракнете върху **да** , за да разрешите архивната пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="04c63-119">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="04c63-120">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="04c63-120">For more information, see:</span></span>
  
- [<span data-ttu-id="04c63-121">Разрешаване на архивни пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="04c63-121">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="04c63-122">Настройване на правила за архивиране и изтриване</span><span class="sxs-lookup"><span data-stu-id="04c63-122">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
