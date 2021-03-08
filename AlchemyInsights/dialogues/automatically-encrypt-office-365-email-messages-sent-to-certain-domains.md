---
title: Автоматично шифроване на имейл съобщения на Office 365, изпратени до определени домейни
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523551"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="c61d7-102">Автоматично шифроване на имейл съобщения на Office 365, изпратени до определени домейни</span><span class="sxs-lookup"><span data-stu-id="c61d7-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="c61d7-103">От [центъра за администриране на Exchange](https://outlook.office365.com/ecp/)изберете " **пощенски поток" > правила**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="c61d7-104">Щракнете върху иконата **нова (+)** и след това щракнете върху **прилагане на шифроване на съобщения в Office 365 и защита на правата към съобщенията**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="c61d7-105">В **име** въведете име за правилото, като например *шифроване на съобщения, изпратени до contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="c61d7-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="c61d7-106">В **прилагане на това правило, ако** изберете **получателя > домейна**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="c61d7-107">Въведете името на домейна, например **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="c61d7-108">Щракнете върху иконата **Add (+)** и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="c61d7-109">До полето **направете следното** щракнете върху **Избери една**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="c61d7-110">В падащото меню **RMS шаблон** изберете **шифроване** и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="c61d7-111">(Ако не виждате тази опция, това означава, че вашият план не включва автоматично шифроване.</span><span class="sxs-lookup"><span data-stu-id="c61d7-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="c61d7-112">Но можете да го добавите.)</span><span class="sxs-lookup"><span data-stu-id="c61d7-112">But you can add it!)</span></span>
9. <span data-ttu-id="c61d7-113">Изберете произволна селекция (от списък с допълнителни селекции, които можете да направите в този момент, като много от тях могат да бъдат оставени с настройката по подразбиране за улеснение).</span><span class="sxs-lookup"><span data-stu-id="c61d7-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="c61d7-114">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="c61d7-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="c61d7-115">Можете винаги да се върнете и да редактирате това правило по-късно.</span><span class="sxs-lookup"><span data-stu-id="c61d7-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="c61d7-116">За повече информация относно създаването на правила за шифроване вижте [определяне на правилата за пощенския поток за шифроване на имейл съобщения в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="c61d7-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>