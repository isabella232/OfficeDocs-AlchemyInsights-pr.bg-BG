---
title: 2681 Attack Simulator в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545715"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="c9f82-102">Атака на тренажор в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="c9f82-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="c9f82-103">Липсва ли ви таен тренажор?</span><span class="sxs-lookup"><span data-stu-id="c9f82-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="c9f82-104">Симулаторът на атаки **изисква Microsoft Defender Office 365 план 2** или Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="c9f82-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="c9f82-105">Симулаторът на **атаки не** е включен в Microsoft Defender за Office 365 план 1, Office 365 Enterprise E3 или Приложения на Microsoft 365 за бизнеса абонаменти.</span><span class="sxs-lookup"><span data-stu-id="c9f82-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="c9f82-106">Акаунтът, който използвате за стартиране на симулирани атаки, изисква разрешения на глобален администратор или администратор на защитата и многофакторно удостоверяване (MFA).</span><span class="sxs-lookup"><span data-stu-id="c9f82-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="c9f82-107">За повече информация относно изискванията за таен тренажор [за атаки вж. тази тема.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="c9f82-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="c9f82-108">Важни неща, които трябва да знаете за **симулации за атака с** парола на Brute Force:</span><span class="sxs-lookup"><span data-stu-id="c9f82-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="c9f82-109">Ако целевият акаунт е разрешен за MFA и паролата е била познана правилно, акаунтът няма да се покаже като компрометиран (вторият фактор за удостоверяване ще бъде непълен).</span><span class="sxs-lookup"><span data-stu-id="c9f82-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="c9f82-110">Файлът с парола не може да бъде по-голям от 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="c9f82-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="c9f82-111">Използвайте по една парола на ред и включете празен ред (връщане на каретата) след последната парола в списъка.</span><span class="sxs-lookup"><span data-stu-id="c9f82-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="c9f82-112">Важни неща, които трябва да знаете за **прикачването на симулации** за фишинг на Spear:</span><span class="sxs-lookup"><span data-stu-id="c9f82-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="c9f82-113">По проект не можете да предоставите стойност по избор за URL адрес на сървъра за **фишинг влизане.**</span><span class="sxs-lookup"><span data-stu-id="c9f82-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="c9f82-114">Ако получателят използва добавката [Разреши](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) съобщението за отчет, за да съобщи за съобщението като фишинг, е възможно да не получавате известия за съобщението (тъй като това е симулирана атака).</span><span class="sxs-lookup"><span data-stu-id="c9f82-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="c9f82-115">Отчети: След като симулираната атака завърши, можете да щракнете върху Подробни данни **за атаката,** за да видите отчета.</span><span class="sxs-lookup"><span data-stu-id="c9f82-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="c9f82-116">За подробни инструкции и нови функции в симулатора на атаки вижте [Симулатор на атаки в Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="c9f82-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
