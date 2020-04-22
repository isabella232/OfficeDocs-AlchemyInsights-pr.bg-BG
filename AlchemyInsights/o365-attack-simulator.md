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
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713455"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="b7c99-102">Симулатор на атаки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="b7c99-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="b7c99-103">Липсва ли симулатор на атака?</span><span class="sxs-lookup"><span data-stu-id="b7c99-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="b7c99-104">Симулатор ът на атаки изисква **План за разширена защита на заплахите 2 на Office (ATP план 2)** или **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="b7c99-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="b7c99-105">Симулатор на атаки **не** е включен в План за защита от заплахи на Office 365 1 (ATP план 1), Office 365 Enterprise E3 или всички приложения на Microsoft 365 за бизнес абонаменти.</span><span class="sxs-lookup"><span data-stu-id="b7c99-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="b7c99-106">Акаунтът, който използвате за стартиране на симулирани атаки изисква разрешения на глобален администратор или администратор на защитата и многофакторно удостоверяване (МВНР).</span><span class="sxs-lookup"><span data-stu-id="b7c99-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="b7c99-107">За повече информация относно изискванията за симулатор на атака вижте [тази тема](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="b7c99-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="b7c99-108">Важни неща, които трябва да знаете за симулации на атака **Brute Force Password:**</span><span class="sxs-lookup"><span data-stu-id="b7c99-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="b7c99-109">Ако целевият акаунт е активирана и паролата е отгатната правилно, акаунтът няма да се показва като компрометирана (вторият фактор за удостоверяване ще бъде непълен).</span><span class="sxs-lookup"><span data-stu-id="b7c99-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="b7c99-110">Файлът с парола не може да бъде по-голям от 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="b7c99-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="b7c99-111">Използвайте по една парола на ред и включете празен ред (връщане на каретата) след последната парола в списъка.</span><span class="sxs-lookup"><span data-stu-id="b7c99-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="b7c99-112">Важни неща, които трябва да знаете за фишинг симулациите **на Spear Phishing:**</span><span class="sxs-lookup"><span data-stu-id="b7c99-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="b7c99-113">По дизайн не можете да предоставите потребителска стойност за URL адрес на сървър за **влизане в фишинг**.</span><span class="sxs-lookup"><span data-stu-id="b7c99-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="b7c99-114">Ако получателят използва [добавката Разрешаване на съобщението](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) за съобщаване за съобщение като фишинг, може да не получавате предупреждения за съобщението (защото това е симулирана атака).</span><span class="sxs-lookup"><span data-stu-id="b7c99-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="b7c99-115">Отчети: След като симулирана атака завърши, можете да щракнете върху **Подробности за атаката,** за да видите отчета.</span><span class="sxs-lookup"><span data-stu-id="b7c99-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="b7c99-116">За подробни инструкции и нови функции в атака [симулатор, вижте Атака симулатор в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="b7c99-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
