---
title: Автоматично преместене на имейл съобщения в архивната пощенска кутия
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
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523603"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="90455-102">Автоматично преместене на имейл съобщения в архивната пощенска кутия</span><span class="sxs-lookup"><span data-stu-id="90455-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="90455-103">Ето как да настроите правила за автоматично преместене на стария имейл на потребител в архивната пощенска кутия:</span><span class="sxs-lookup"><span data-stu-id="90455-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="90455-104">Отидете на страницата за защита за управление на данни в [**съответствие &**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >    >   , за да проверите дали е разрешена пощенска кутия за архивиране за потребителя.</span><span class="sxs-lookup"><span data-stu-id="90455-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="90455-105">Ако не е, щракнете върху **Разреши** , а след това **да** в полето за предупреждение.</span><span class="sxs-lookup"><span data-stu-id="90455-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="90455-106">Отидете в [**центъра за администриране на Exchange > управление на съответствието > етикети за съхранение**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="90455-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="90455-107">Изберете иконата +, след което изберете **автоматично прилагане към цялата пощенска кутия**.</span><span class="sxs-lookup"><span data-stu-id="90455-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="90455-108">Присвояване на име на етикет за съхранение и изберете **преминаване към архивиране**.</span><span class="sxs-lookup"><span data-stu-id="90455-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="90455-109">За периода на съхранение въведете часа, който искате, като например 90 дни.</span><span class="sxs-lookup"><span data-stu-id="90455-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="90455-110">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="90455-110">Click **Save**.</span></span>
5. <span data-ttu-id="90455-111">Сега създайте правила за съхранение: изберете **правила за съхранение**, изберете иконата, за да добавите нови правила.</span><span class="sxs-lookup"><span data-stu-id="90455-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="90455-112">Дайте име на правилата за съхранение, след което щракнете и превъртете, за да намерите и добавите етикета за съхранение, който току-що създадохте.</span><span class="sxs-lookup"><span data-stu-id="90455-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="90455-113">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="90455-113">Click **Save**.</span></span>
7. <span data-ttu-id="90455-114">И накрая, приложете правилата за съхранение към пощенската кутия на потребителя: все още в центъра за администриране на Exchange, отидете на  >  **пощенските кутии** на получателите.</span><span class="sxs-lookup"><span data-stu-id="90455-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="90455-115">Изберете всички потребители, за които искате да приложите правилата, след което изберете **Редактиране** (иконата на молив).</span><span class="sxs-lookup"><span data-stu-id="90455-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="90455-116">В диалоговия прозорец щракнете върху **функции за пощенската кутия**.</span><span class="sxs-lookup"><span data-stu-id="90455-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="90455-117">Под **правила за съхранение** Приложете правилата, които току-що създадохте, > **запишете**.</span><span class="sxs-lookup"><span data-stu-id="90455-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="90455-118">За инструкции за прилагане на правилата към всички потребители вижте [прилагане на правила за съхранение към пощенски кутии](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="90455-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
