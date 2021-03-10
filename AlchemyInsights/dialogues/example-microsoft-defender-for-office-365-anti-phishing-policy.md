---
title: Например правила за Microsoft Defender за Office 365 за анти-фишинг
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692619"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="d1adc-102">Например правила за Microsoft Defender за Office 365 за анти-фишинг</span><span class="sxs-lookup"><span data-stu-id="d1adc-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="d1adc-103">Тези настройки разрешават правила, наречени *Domain и CEO*.</span><span class="sxs-lookup"><span data-stu-id="d1adc-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="d1adc-104">Тези правила предоставят защита на потребителите и домейните от въплъщаване и след това прилага правилата към всички имейли, получени от потребители в домейна.</span><span class="sxs-lookup"><span data-stu-id="d1adc-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="d1adc-105">Първо, добавете следната информация, за да създадете правилата:</span><span class="sxs-lookup"><span data-stu-id="d1adc-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="d1adc-106">**Име**: **Описание** на домейни и главен изпълнителен директор: гарантира, че главният изпълнителен директор и вашият домейн не се представят като превъплъщават.</span><span class="sxs-lookup"><span data-stu-id="d1adc-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="d1adc-107">**Приложено към**: изберете **домейна на получателя**.</span><span class="sxs-lookup"><span data-stu-id="d1adc-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="d1adc-108">Под **някое от тези** изберете **избор** и след това изберете домейн.</span><span class="sxs-lookup"><span data-stu-id="d1adc-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="d1adc-109">Изберете **+ Add**.</span><span class="sxs-lookup"><span data-stu-id="d1adc-109">Select **+ Add**.</span></span> <span data-ttu-id="d1adc-110">Поставете отметка в квадратчето до името на домейна в списъка (например *contoso.com*) и след това изберете **Добави**.</span><span class="sxs-lookup"><span data-stu-id="d1adc-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="d1adc-111">Изберете **Готово**.</span><span class="sxs-lookup"><span data-stu-id="d1adc-111">Select **Done**.</span></span>
- <span data-ttu-id="d1adc-112">След създаването на правилата можете да прецизирате правилата с помощта на следните опции:</span><span class="sxs-lookup"><span data-stu-id="d1adc-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="d1adc-113">**Добавете потребители, за да защитите:** За този пример Добавете имейл адреса на изпълнителния директор най-малко.</span><span class="sxs-lookup"><span data-stu-id="d1adc-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="d1adc-114">**Добавете домейни за защита**: Добавете организационния домейн, който включва Office на изпълнителния директор.</span><span class="sxs-lookup"><span data-stu-id="d1adc-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="d1adc-115">**Изберете действия**: **ако имейлът е изпратен от неолицетворяван потребител**, изберете **пренасочване на съобщение към друг имейл адрес** и след това въведете имейл адреса на администратора по защитата (например *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="d1adc-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="d1adc-116">**Ако имейлът е изпратен от домейн с имена**, изберете **поставяне под карантина на съобщението**.</span><span class="sxs-lookup"><span data-stu-id="d1adc-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="d1adc-117">**Интелигентност на пощенските кутии**: по подразбиране тази опция е избрана, когато създавате нова политика против фишинг.</span><span class="sxs-lookup"><span data-stu-id="d1adc-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="d1adc-118">Оставете тази настройка **включена** за най-добри резултати.</span><span class="sxs-lookup"><span data-stu-id="d1adc-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="d1adc-119">**Добавяне на надеждни податели и домейни:** За този пример не се дефинират замествания.</span><span class="sxs-lookup"><span data-stu-id="d1adc-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="d1adc-120">След като сте прегледали настройките си, изберете **Създаване на тези правила** или **Запиши** по подходящ начин.</span><span class="sxs-lookup"><span data-stu-id="d1adc-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="d1adc-121">За да научите повече, вижте [правила за защита от фишинг в Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="d1adc-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
