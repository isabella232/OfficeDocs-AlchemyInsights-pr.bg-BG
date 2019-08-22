---
title: Поток имейл не се изпраща
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530851"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="507a5-102">Поток имейл не се изпраща за SharePoint списък или библиотека</span><span class="sxs-lookup"><span data-stu-id="507a5-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="507a5-103">Имейл от работни потоци, които не са изпратени до всички потребители или само определени потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.</span><span class="sxs-lookup"><span data-stu-id="507a5-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="507a5-104">Проверете дали потребителят съществува в група за разрешения на **Всички хора** (списък с потребителска информация) за тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="507a5-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="507a5-105">Проба директно URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="507a5-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="507a5-106">Ако потребителят не съществува, се уверете, че потребителят е подписан в страницата.</span><span class="sxs-lookup"><span data-stu-id="507a5-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="507a5-107">Ако е външен потребител, се уверете, че техните покана е била приета.</span><span class="sxs-lookup"><span data-stu-id="507a5-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="507a5-108">Ако потребителят съществува в групата разрешения, се уверете, че имейл адресът е правилен.</span><span class="sxs-lookup"><span data-stu-id="507a5-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="507a5-109">Ако потребителите имейл адрес не е настроен тук, след това създайте примерно предупреждение за този потребител, който принуждава синхронизиране на този акаунт от потребителски профили на SharePoint към тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="507a5-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="507a5-110">Имейл от работни потоци са изпратени до администраторите на колекцията сайтове, но не на други потребители и видите грешка **HTTP Забранения да <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="507a5-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="507a5-111">Вижте [Отказан достъп, когато изпращате имейл на SharePoint група](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="507a5-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="507a5-112">Също така Уверете се че функция на колекция сайтове **ограничен достъп потребител разрешение lockdown режим** не е активен.</span><span class="sxs-lookup"><span data-stu-id="507a5-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="507a5-113">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="507a5-113">Related topics</span></span>
<span data-ttu-id="507a5-114">Искате ли да опитате Microsoft поток в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="507a5-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="507a5-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="507a5-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="507a5-116">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="507a5-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


