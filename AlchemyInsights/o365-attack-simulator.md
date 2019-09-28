---
title: 2681 симулатор на атака в Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305321"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="7405e-102">Симулатор атака в офис 365</span><span class="sxs-lookup"><span data-stu-id="7405e-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="7405e-103">Няма ли симулатор на атака?</span><span class="sxs-lookup"><span data-stu-id="7405e-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="7405e-104">Атака симулатор изисква **Office 365 Advanced заплаха защита план 2 (ATP план 2)** или **Office 365 Enterprise**Е5.</span><span class="sxs-lookup"><span data-stu-id="7405e-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="7405e-105">Атака симулатор **не** е включен в Office 365 Advanced заплаха защита план 1 (ATP план 1), Office 365 Enterprise Е3 или всеки Office 365 бизнес абонаменти.</span><span class="sxs-lookup"><span data-stu-id="7405e-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="7405e-106">Акаунтът, който използвате за стартиране на симулираните атаки, изисква глобален администратор или разрешения на администратора на защитата и многофакторно удостоверяване (МФП).</span><span class="sxs-lookup"><span data-stu-id="7405e-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="7405e-107">За повече информация относно атака симулатор изисквания вижте [тази тема](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="7405e-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="7405e-108">Важни неща, които да знаят за симулациите на атаката на **Бруталите** :</span><span class="sxs-lookup"><span data-stu-id="7405e-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="7405e-109">Ако целевият акаунт има МФП разрешена и паролата е бил отгатнат правилно, акаунтът няма да се покаже като компрометиран (Вторият фактор за удостоверяване ще бъде непълен).</span><span class="sxs-lookup"><span data-stu-id="7405e-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="7405e-110">Файлът с паролата не може да бъде по-голям от 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="7405e-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="7405e-111">Използвайте една парола на ред и включете празен ред (връщане на превоз) след последната парола в списъка.</span><span class="sxs-lookup"><span data-stu-id="7405e-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="7405e-112">Важни неща, които да знаете за **копие фишинг** придават симулации:</span><span class="sxs-lookup"><span data-stu-id="7405e-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="7405e-113">По дизайн не можете да предоставите стойност по избор за **URL адреса на сървъра за влизане в фишинг**.</span><span class="sxs-lookup"><span data-stu-id="7405e-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="7405e-114">Ако получателят използва [опцията разрешаване на добавката за отчет](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , за да съобщи съобщението като фишинг, може да не получавате предупреждения за съобщението (защото това е симулирана атака).</span><span class="sxs-lookup"><span data-stu-id="7405e-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="7405e-115">Отчети: след като симулираната атака завърши, можете да щракнете върху **подробности за атаката** , за да видите отчета.</span><span class="sxs-lookup"><span data-stu-id="7405e-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="7405e-116">За подробни инструкции и нови функции в атака симулатор, вижте [симулатор атака в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="7405e-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
