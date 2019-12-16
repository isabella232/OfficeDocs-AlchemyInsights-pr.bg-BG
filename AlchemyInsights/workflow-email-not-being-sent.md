---
title: Имейл работният поток не се изпраща
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049362"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="a4646-102">Имейл работен поток не се изпраща за списък или библиотека на SharePoint</span><span class="sxs-lookup"><span data-stu-id="a4646-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="a4646-103">Имейл от работни потоци не се изпращат до всички потребители или само конкретни потребители, или виждате грешка **имейл съобщението не може да бъде изпратено. Уверете се, че имейлът има валиден получател**.</span><span class="sxs-lookup"><span data-stu-id="a4646-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="a4646-104">Проверете дали потребителят съществува в групата " **всички хора** разрешения" (списък с потребителски информация) за тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="a4646-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="a4646-105">Примерен Директен URL адрес:<tenant>https://.<sitename>SharePoint.com/Sites//_layouts/15/kari.Lap? Членове на групата = 0</span><span class="sxs-lookup"><span data-stu-id="a4646-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="a4646-106">Ако потребителят не съществува, уверете се, че потребителят е влязъл в страницата.</span><span class="sxs-lookup"><span data-stu-id="a4646-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="a4646-107">Ако е външен потребител, уверете се, че поканата им е приета.</span><span class="sxs-lookup"><span data-stu-id="a4646-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="a4646-108">Ако потребителят съществува в групата с разрешения, уверете се, че имейл адресът е правилен.</span><span class="sxs-lookup"><span data-stu-id="a4646-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="a4646-109">Ако потребителят имейл адрес не е зададен тук, след това създайте примерен сигнал за този потребител, който принуждава синхронизирането на този потребителски акаунт от потребителски профили на SharePoint в тази колекция от сайтове.</span><span class="sxs-lookup"><span data-stu-id="a4646-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="a4646-110">Имейл от работни потоци се изпращат на администраторите на колекцията от сайтове, но не и на други потребители и да видите грешка **http забранено да <span>HTTPS:</span>//_vti_bin/клиент.ксвк.сп.утилитиес.утилити.сендемаил**.</span><span class="sxs-lookup"><span data-stu-id="a4646-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="a4646-111">Вижте [достъп отказан, когато изпращате имейл до група на SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="a4646-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="a4646-112">Също така Уверете се, че **ограничен достъп потребител разрешение режим заключване** сайт колекция не е активен.</span><span class="sxs-lookup"><span data-stu-id="a4646-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="a4646-113">Сродни теми</span><span class="sxs-lookup"><span data-stu-id="a4646-113">Related topics</span></span>
<span data-ttu-id="a4646-114">Искате ли да опитате Microsoft Flow в SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="a4646-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="a4646-115">Създаване на поток</span><span class="sxs-lookup"><span data-stu-id="a4646-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="a4646-116">SharePoint и поток</span><span class="sxs-lookup"><span data-stu-id="a4646-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


