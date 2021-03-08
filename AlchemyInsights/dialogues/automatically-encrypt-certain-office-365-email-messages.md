---
title: Автоматично шифроване на определени имейл съобщения на Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523559"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="89bc5-102">Автоматично шифроване на определени имейл съобщения на Office 365</span><span class="sxs-lookup"><span data-stu-id="89bc5-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="89bc5-103">Можете автоматично да шифровате съобщения, изпратени от потребители до определени външни хора или организации.</span><span class="sxs-lookup"><span data-stu-id="89bc5-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="89bc5-104">За да направите това, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="89bc5-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="89bc5-105">От [центъра за администриране на Exchange](https://outlook.office365.com/ecp/)изберете " **пощенски поток" > правила**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="89bc5-106">Щракнете върху иконата **нова (+)** и след това щракнете върху **прилагане на шифроване на съобщения в Office 365 и защита на правата към съобщенията**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="89bc5-107">В **име** въведете име за правилото, като например *шифроване на съобщения, изпратени до DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="89bc5-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="89bc5-108">В **прилагане на това правило, ако** изберете **получателя > е този човек**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="89bc5-109">В диалоговия прозорец **избор на членове** изберете името на лицето, на което искате да се приложи правилото за шифроване, и след това щракнете върху **Добави**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="89bc5-110">Когато сте готови с добавянето на потребители, щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="89bc5-111">До полето **направете следното** щракнете върху **Избери една**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="89bc5-112">В падащото меню **RMS шаблон** изберете **шифроване** и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="89bc5-113">(Ако не виждате тази опция, това означава, че вашият план не включва автоматично шифроване.</span><span class="sxs-lookup"><span data-stu-id="89bc5-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="89bc5-114">Но можете да го добавите.)</span><span class="sxs-lookup"><span data-stu-id="89bc5-114">But you can add it!)</span></span>
9. <span data-ttu-id="89bc5-115">Изберете произволна селекция (от списък с допълнителни селекции, които можете да направите в този момент, като много от тях могат да бъдат оставени с настройката по подразбиране за улеснение).</span><span class="sxs-lookup"><span data-stu-id="89bc5-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="89bc5-116">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="89bc5-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="89bc5-117">Можете винаги да се върнете и да редактирате това правило по-късно.</span><span class="sxs-lookup"><span data-stu-id="89bc5-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="89bc5-118">За повече информация относно създаването на правила за шифроване вижте [определяне на правилата за пощенския поток за шифроване на имейл съобщения в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="89bc5-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

