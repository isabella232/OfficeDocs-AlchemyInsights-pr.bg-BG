---
title: Управление на външни настройки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294143"
---
# <a name="managing-external-settings"></a><span data-ttu-id="8f478-102">Управление на външни настройки</span><span class="sxs-lookup"><span data-stu-id="8f478-102">Managing External Settings</span></span>

<span data-ttu-id="8f478-103">**Известие**</span><span class="sxs-lookup"><span data-stu-id="8f478-103">**Announcement**</span></span>

- <span data-ttu-id="8f478-104">Отхвърляне [на поддръжката на WebView за влизане от Google, започваща на 4 януари, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span><span class="sxs-lookup"><span data-stu-id="8f478-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="8f478-105">Проверете дали вашите приложения са засегнати, като следвате указанията на Google относно проверката за съвместимост</span><span class="sxs-lookup"><span data-stu-id="8f478-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="8f478-106">Уверете се, че използвате System WebView или браузър на системата, когато влизате в своите потребители с потребителски акаунти за Google</span><span class="sxs-lookup"><span data-stu-id="8f478-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="8f478-107">**Управление на настройките за покана**</span><span class="sxs-lookup"><span data-stu-id="8f478-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="8f478-108">Уверете се, че сте [конфигурирали настройките за външно сътрудничество](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) , за да разрешите на подходящите хора да изпратят покани.</span><span class="sxs-lookup"><span data-stu-id="8f478-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="8f478-109">**Управление на разрешенията за достъп на потребител за гости**</span><span class="sxs-lookup"><span data-stu-id="8f478-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="8f478-110">Глобалните администратори могат да управляват разрешенията за достъп на гости в указателя през портала на Azure, като конфигурират разрешенията за достъп на гости на страницата с настройки за външно сътрудничество.</span><span class="sxs-lookup"><span data-stu-id="8f478-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="8f478-111">[Научете повече за тази настройка](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8f478-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="8f478-112">Ако искате гостите ви да получат достъп до приложения като Teams или SharePoint, потвърдете, че сте конфигурирали тези приложения, за да разрешите достъп на гости.</span><span class="sxs-lookup"><span data-stu-id="8f478-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="8f478-113">Научете повече за [настройките за Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) и [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="8f478-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="8f478-114">**Конфигуриране на покани:**</span><span class="sxs-lookup"><span data-stu-id="8f478-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="8f478-115">Разрешаване на външното сътрудничество на B2B и управление кой може да кани гости</span><span class="sxs-lookup"><span data-stu-id="8f478-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8f478-116">Разрешаване или блокиране на покани към потребители от определени организации</span><span class="sxs-lookup"><span data-stu-id="8f478-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="8f478-117">**Конфигуриране на разрешени доставчици на самоличност:**</span><span class="sxs-lookup"><span data-stu-id="8f478-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="8f478-118">Google федерация</span><span class="sxs-lookup"><span data-stu-id="8f478-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8f478-119">Директна федерация</span><span class="sxs-lookup"><span data-stu-id="8f478-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="8f478-120">Имейл удостоверяване с еднократна парола</span><span class="sxs-lookup"><span data-stu-id="8f478-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
