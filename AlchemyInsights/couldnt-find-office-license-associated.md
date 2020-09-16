---
title: Поправянето на приложения на Microsoft 365 не можа да намери асоциираното съобщение на Office лицензи
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747684"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="dcef0-102">Поправянето на приложенията на Microsoft 365 "не можа да намери асоциираните лицензи за Office"</span><span class="sxs-lookup"><span data-stu-id="dcef0-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="dcef0-103">Ако получите това съобщение, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="dcef0-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="dcef0-104">Проверете защитната стена, антивирусния софтуер и настройките за прокси сървър, за да потвърдите, че не блокират достъпа до интернет за приложенията на Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="dcef0-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="dcef0-105">Вижте [диапазони от URL и IP адреси за Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="dcef0-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="dcef0-106">Премахнете и [повторно Дайте лиценза за Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) за засегнатия потребител.</span><span class="sxs-lookup"><span data-stu-id="dcef0-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="dcef0-107">Отворете приложение от [Office и излезте от всички](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) съществуващи потребителски акаунти.</span><span class="sxs-lookup"><span data-stu-id="dcef0-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="dcef0-108">Отидете на настройки на Windows > **акаунти**за  >  **имейл & акаунти**и премахнете всички служебни акаунти, с изключение на засегнатия акаунт.</span><span class="sxs-lookup"><span data-stu-id="dcef0-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="dcef0-109">Отидете на настройки на Windows > **акаунтите**за  >  **достъп до работно място или учебно заведение**и прекъснете връзката на всички служебни акаунти с изключение на засегнат</span><span class="sxs-lookup"><span data-stu-id="dcef0-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="dcef0-110">Нулиране на състоянието на активиране на Office.</span><span class="sxs-lookup"><span data-stu-id="dcef0-110">Reset the Office activation state.</span></span> <span data-ttu-id="dcef0-111">[Научете как](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="dcef0-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="dcef0-112">[Влезете](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) с помощта на засегнатия потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="dcef0-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="dcef0-113">За допълнителни решения за отстраняване на неизправности вижте [нелицензиран продукт и грешки при активиране в Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="dcef0-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>