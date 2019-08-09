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
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270661"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="f01ab-102">Поток имейл не се изпраща</span><span class="sxs-lookup"><span data-stu-id="f01ab-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="f01ab-103">Имейл от работни потоци, които не са изпратени до всички потребители или само определени потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.</span><span class="sxs-lookup"><span data-stu-id="f01ab-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="f01ab-104">Проверете дали потребителят съществува в група за разрешения на **Всички хора** (списък с потребителска информация) за тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="f01ab-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="f01ab-105">Проба директно URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="f01ab-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="f01ab-106">Ако потребителят не съществува, се уверете, че потребителят е подписан в страницата.</span><span class="sxs-lookup"><span data-stu-id="f01ab-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="f01ab-107">Ако е външен потребител, се уверете, че техните покана е била приета.</span><span class="sxs-lookup"><span data-stu-id="f01ab-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="f01ab-108">Ако потребителят съществува в групата разрешения, се уверете, че имейл адресът е правилен.</span><span class="sxs-lookup"><span data-stu-id="f01ab-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="f01ab-109">Ако потребителите имейл адрес не е настроен тук, след това създайте примерно предупреждение за този потребител, който принуждава синхронизиране на този акаунт от потребителски профили на SharePoint към тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="f01ab-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="f01ab-110">Имейл от работни потоци са изпратени до администраторите на колекцията сайтове, но не на други потребители и видите грешка \*\*HTTP Забранения да <spam> <spam> \*\* <spam> <spam>.</span><span class="sxs-lookup"><span data-stu-id="f01ab-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

    <span data-ttu-id="f01ab-111">Вижте [Отказан достъп, когато се изпраща имейл до групите](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="f01ab-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="f01ab-112">Също така Уверете се че функция на колекция сайтове **ограничен достъп потребител разрешение lockdown режим** не е активен.</span><span class="sxs-lookup"><span data-stu-id="f01ab-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="f01ab-113">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="f01ab-113">Related topics</span></span>
<span data-ttu-id="f01ab-114">Искате ли да опитате Microsoft поток в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="f01ab-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="f01ab-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="f01ab-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f01ab-116">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="f01ab-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


