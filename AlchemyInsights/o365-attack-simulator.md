---
title: 2681 атака симулатор в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 3dae4768ca62757ce7f92dfc527078c963d72742
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506727"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b89a9-102">Симулатор на атаки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b89a9-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b89a9-103">Липсва ли ви симулатор на атака?</span><span class="sxs-lookup"><span data-stu-id="b89a9-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b89a9-104">Атака симулатор изисква **Office 365 разширено заплаха защита план 2 (ATP план 2)** или **Office 365 предприятие E5**.</span><span class="sxs-lookup"><span data-stu-id="b89a9-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b89a9-105">Атака симулатор **не** е включена в Office 365 Разширено заплаха защита план 1 (ATP план 1), Office 365 Enterprise E3 или приложения на Microsoft 365 за бизнес абонаменти.</span><span class="sxs-lookup"><span data-stu-id="b89a9-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b89a9-106">Акаунтът, който използвате за стартиране на симулирани атаки, изисква глобален администратор или администратор на защитата разрешения и многофакторно удостоверяване (МРНП).</span><span class="sxs-lookup"><span data-stu-id="b89a9-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b89a9-107">За повече информация относно изискванията на симулатора на атака вижте [тази тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b89a9-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="b89a9-108">Важни неща, които трябва да знаете за **Brute Force Парола** атака симулации:</span><span class="sxs-lookup"><span data-stu-id="b89a9-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b89a9-109">Ако целевият акаунт е активиран и паролата е познан, акаунтът няма да се покаже като компрометиран (вторият фактор за удостоверяване ще бъде непълна).</span><span class="sxs-lookup"><span data-stu-id="b89a9-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b89a9-110">Файлът с парола не може да бъде по-голям от 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="b89a9-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b89a9-111">Използвайте една парола на ред и включете празен ред (връщане на карета) след последната парола в списъка.</span><span class="sxs-lookup"><span data-stu-id="b89a9-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b89a9-112">Важни неща, които трябва да знаете за **Spear Phishing** приложете симулации:</span><span class="sxs-lookup"><span data-stu-id="b89a9-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b89a9-113">По дизайн не можете да предоставите потребителска стойност за **фишинг url адрес на сървъра за влизане.**</span><span class="sxs-lookup"><span data-stu-id="b89a9-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b89a9-114">Ако получателят използва [добавката Разрешаване на съобщение](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) за отчет, за да съобщите съобщението като фишинг, може да не получавате предупреждения за съобщението (защото това е симулирана атака).</span><span class="sxs-lookup"><span data-stu-id="b89a9-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b89a9-115">Отчети: След като симулираната атака завърши, можете да кликнете върху Подробности за **атака,** за да видите отчета.</span><span class="sxs-lookup"><span data-stu-id="b89a9-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b89a9-116">За подробни инструкции и нови функции в атака симулатор вижте [атака симулатор в Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="b89a9-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
