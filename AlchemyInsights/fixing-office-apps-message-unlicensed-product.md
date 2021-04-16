---
title: Не може да се активира Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812561"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="dcc7e-102">Не може да се активира Office</span><span class="sxs-lookup"><span data-stu-id="dcc7e-102">Unable to activate Office</span></span>

- <span data-ttu-id="dcc7e-103">Проверете дали срокът на абонамента ви не е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="dcc7e-104">Уверете се, че имате абонамент, който позволява клиентски лицензи, като например Office 365 Business или Business Premium, и се уверете, [че потребителят има присвоен лиценз.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="dcc7e-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="dcc7e-105">Уверете се, че потребителят влиза в Office със същия акаунт, на който е присвоен лицензът.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="dcc7e-106">Проверете [Страницата за състояние на услугата Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), за да видите дали няма някакви известни проблеми с услугата.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="dcc7e-107">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те не блокират достъпа на приложенията на Microsoft 365 до интернет.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="dcc7e-108">Вижте [Диапазони на URL и IP адреси за Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Диапазони от URL и IP адреси за Office 365").</span><span class="sxs-lookup"><span data-stu-id="dcc7e-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="dcc7e-109">**Съвет** На компютри с Windows можем да диагностицираме и автоматично да коригираме няколко често срещани проблема с влизането в Office.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="dcc7e-110">Изтеглете и стартирайте  **[помощника за поддръжка и възстановяване на Microsoft,](https://aka.ms/SaRA-OfficeSignInScenario)** за да използвате нашия автоматизиран инструмент.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="dcc7e-111">Използвайте следните действия за отстраняване на проблеми:</span><span class="sxs-lookup"><span data-stu-id="dcc7e-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="dcc7e-112">Отворете приложение на Office и [излезте](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) от всички съществуващи потребителски акаунти.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="dcc7e-113">[Премахнете](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [дайте повторно](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лиценз за Office, а след това [влезте в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) като използвате засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="dcc7e-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="dcc7e-114">Изпълнение на [Програмата за отстраняване на проблеми при активиране](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="dcc7e-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="dcc7e-115">Нулиране на състоянието на активиране на Office</span><span class="sxs-lookup"><span data-stu-id="dcc7e-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Нулиране на състоянието на активиране на Office")
- [<span data-ttu-id="dcc7e-116">Извършване на онлайн поправка на Office</span><span class="sxs-lookup"><span data-stu-id="dcc7e-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="dcc7e-117">За допълнителни решения за отстраняване на проблеми вижте:</span><span class="sxs-lookup"><span data-stu-id="dcc7e-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="dcc7e-118">Грешки поради нелицензиран продукт и грешки при активиране на Office</span><span class="sxs-lookup"><span data-stu-id="dcc7e-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="dcc7e-119">Грешка при активиране на Office. "За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"</span><span class="sxs-lookup"><span data-stu-id="dcc7e-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)