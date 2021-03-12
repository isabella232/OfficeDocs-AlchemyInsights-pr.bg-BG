---
title: Автоматично шифроване на определени имейл съобщения от Office 365
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
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743367"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="14c07-102">Автоматично шифроване на определени имейл съобщения от Office 365</span><span class="sxs-lookup"><span data-stu-id="14c07-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="14c07-103">От [центъра за администриране на Exchange](https://outlook.office365.com/ecp/)изберете " **пощенски поток" > правила**.</span><span class="sxs-lookup"><span data-stu-id="14c07-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="14c07-104">Щракнете върху иконата **нова (+)** и след това щракнете върху **прилагане на шифроване на съобщения в Office 365 и защита на правата към съобщенията**.</span><span class="sxs-lookup"><span data-stu-id="14c07-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="14c07-105">В **име** въведете име за правилото, като например *шифроване на всички съобщения*.</span><span class="sxs-lookup"><span data-stu-id="14c07-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="14c07-106">В **прилагане на това правило, ако** изберете **[Приложи към всички съобщения]**.</span><span class="sxs-lookup"><span data-stu-id="14c07-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="14c07-107">До полето **направете следното** щракнете върху **Избери една**.</span><span class="sxs-lookup"><span data-stu-id="14c07-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="14c07-108">В падащото меню **RMS шаблон** изберете **шифроване** и след това щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="14c07-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="14c07-109">(Ако не виждате тази опция, това означава, че вашият план не включва автоматично шифроване.</span><span class="sxs-lookup"><span data-stu-id="14c07-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="14c07-110">Но можете да го добавите.)</span><span class="sxs-lookup"><span data-stu-id="14c07-110">But you can add it!)</span></span>
7. <span data-ttu-id="14c07-111">Поставете отметка в квадратчето Проверявай **това правило с ниво на тежест** и след това изберете желаното от вас ниво.</span><span class="sxs-lookup"><span data-stu-id="14c07-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="14c07-112">Ако вашата фирма има договорни задължения да изпраща всички шифровани имейли, препоръчвам ви да настроите нивото на **високо**.</span><span class="sxs-lookup"><span data-stu-id="14c07-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="14c07-113">Под **изберете модел за това правило** щракнете върху **прилагане**.</span><span class="sxs-lookup"><span data-stu-id="14c07-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="14c07-114">Изберете произволна селекция (от списък с допълнителни селекции, които можете да направите в този момент, като много от тях могат да бъдат оставени с настройката по подразбиране за улеснение).</span><span class="sxs-lookup"><span data-stu-id="14c07-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="14c07-115">Щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="14c07-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="14c07-116">Можете винаги да се върнете и да редактирате това правило по-късно.</span><span class="sxs-lookup"><span data-stu-id="14c07-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="14c07-117">За повече информация относно създаването на правила за шифроване вижте [определяне на правилата за пощенския поток за шифроване на имейл съобщения в Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="14c07-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

