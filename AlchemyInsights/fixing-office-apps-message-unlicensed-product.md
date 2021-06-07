---
title: Не може да се Office
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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798669"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="8e40a-102">Не може да се Office</span><span class="sxs-lookup"><span data-stu-id="8e40a-102">Unable to activate Office</span></span>

<span data-ttu-id="8e40a-103">**Забележка:** Ако използвате по-стара версия на Windows (Например Windows 7), уверете се, че TLS 1.2 е разрешен като по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="8e40a-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="8e40a-104">За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows.</span><span class="sxs-lookup"><span data-stu-id="8e40a-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="8e40a-105">Проверете дали срокът на абонамента ви не е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="8e40a-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="8e40a-106">Уверете се, че имате абонамент, който позволява клиентски лицензи, като Office 365 Business или Бизнес Premium, и се уверете, че потребителят [има присвоен лиценз](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="8e40a-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="8e40a-107">Уверете се, че потребителят влиза в Office със същия акаунт, на който е присвоен лицензът.</span><span class="sxs-lookup"><span data-stu-id="8e40a-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="8e40a-108">Проверете [Страницата за състояние на услугата Office 365](/office365/enterprise/view-service-health), за да видите дали няма някакви известни проблеми с услугата.</span><span class="sxs-lookup"><span data-stu-id="8e40a-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="8e40a-109">Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те Microsoft 365 блокират достъпа на приложенията до интернет.</span><span class="sxs-lookup"><span data-stu-id="8e40a-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="8e40a-110">Вижте [Диапазони на URL и IP адреси за Office 365](/office365/enterprise/urls-and-ip-address-ranges "Диапазони от URL и IP адреси за Office 365").</span><span class="sxs-lookup"><span data-stu-id="8e40a-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="8e40a-111">**Съвет** На Windows компютри можем да диагностицираме и автоматично да коригираме няколко често срещани Office за влизане.</span><span class="sxs-lookup"><span data-stu-id="8e40a-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8e40a-112">Изтеглете и стартирайте **[microsoft Помощник за поддръжка и възстановяване,](https://aka.ms/SaRA-OfficeSignInScenario)** за да използвате нашия автоматизиран инструмент.</span><span class="sxs-lookup"><span data-stu-id="8e40a-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8e40a-113">Използвайте следните действия за отстраняване на проблеми:</span><span class="sxs-lookup"><span data-stu-id="8e40a-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="8e40a-114">Отворете приложение на Office и [излезте](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) от всички съществуващи потребителски акаунти.</span><span class="sxs-lookup"><span data-stu-id="8e40a-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="8e40a-115">[Премахнете](/microsoft-365/admin/manage/remove-licenses-from-users) и [дайте повторно](/microsoft-365/admin/manage/assign-licenses-to-users) лиценз за Office, а след това [влезте в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) като използвате засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="8e40a-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="8e40a-116">Изпълнение на [Програмата за отстраняване на проблеми при активиране](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="8e40a-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="8e40a-117">Нулиране на състоянието на активиране на Office</span><span class="sxs-lookup"><span data-stu-id="8e40a-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Нулиране на Office на активиране")
- [<span data-ttu-id="8e40a-118">Извършване на онлайн поправка на Office</span><span class="sxs-lookup"><span data-stu-id="8e40a-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="8e40a-119">За допълнителни решения за отстраняване на проблеми вижте:</span><span class="sxs-lookup"><span data-stu-id="8e40a-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="8e40a-120">Грешки поради нелицензиран продукт и грешки при активиране на Office</span><span class="sxs-lookup"><span data-stu-id="8e40a-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="8e40a-121">Грешка при активиране на Office. "За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"</span><span class="sxs-lookup"><span data-stu-id="8e40a-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)