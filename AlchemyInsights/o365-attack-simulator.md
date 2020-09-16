---
title: Симулатор за атаки на 2681 в Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759208"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="8ccc3-102">Симулатор за атаки в Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8ccc3-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="8ccc3-103">Липсващ симулатор за атаки ли сте?</span><span class="sxs-lookup"><span data-stu-id="8ccc3-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="8ccc3-104">Симулаторът за атаки изисква **office 365 Advanced Protection Plan 2 (ATP план 2)** или **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="8ccc3-105">Симулаторът за атаки **не** е включен в Office 365 Advanced план за защита от заплахи 1 (ATP план 1), Office 365 Enterprise E3 или Microsoft 365 приложения за бизнес абонаменти.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="8ccc3-106">Акаунтът, който използвате, за да стартирате симулираните атаки, изисква глобален администратор или разрешения на администратора на защитата и многофакторно удостоверяване (МВНР).</span><span class="sxs-lookup"><span data-stu-id="8ccc3-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="8ccc3-107">За повече информация относно изискванията за симулатор на атаки вижте [тази тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="8ccc3-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="8ccc3-108">Важни неща, които трябва да знаете за симулационните симулации за атаки с **парола на груба сила**</span><span class="sxs-lookup"><span data-stu-id="8ccc3-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="8ccc3-109">Ако целевият акаунт има активиран и паролата е отгатната правилно, акаунтът няма да се показва като компрометиран (Вторият фактор за удостоверяване ще бъде непълен).</span><span class="sxs-lookup"><span data-stu-id="8ccc3-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="8ccc3-110">Файлът с парола не може да е по-голям от 10 МБ.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="8ccc3-111">Използвайте една парола на ред и включвайте празен ред (връщане на превоз) след последната парола в списъка.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="8ccc3-112">Важни неща, които трябва да знаете за **копието на фишинг** прикачване на симулации:</span><span class="sxs-lookup"><span data-stu-id="8ccc3-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="8ccc3-113">По проект не можете да предоставите стойност по избор за **URL адрес на фишинг сървъра за влизане**.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="8ccc3-114">Ако получател използва [добавката разрешаване на съобщение за отчет](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , за да съобщи съобщението като фишинг, е възможно да не получавате предупреждения за съобщението (защото това е симулация на атака).</span><span class="sxs-lookup"><span data-stu-id="8ccc3-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="8ccc3-115">Отчети: след като симулираната атака завърши, можете да щракнете върху **подробности за атака** , за да видите отчета.</span><span class="sxs-lookup"><span data-stu-id="8ccc3-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="8ccc3-116">За подробни инструкции и нови функции в симулатора за атаки вижте [симулатор за атаки в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="8ccc3-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
