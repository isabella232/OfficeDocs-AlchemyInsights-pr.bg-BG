---
title: Изтриване на клиент
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564385"
---
# <a name="delete-tenant"></a><span data-ttu-id="c0b9c-102">Изтриване на клиент</span><span class="sxs-lookup"><span data-stu-id="c0b9c-102">Delete tenant</span></span>

<span data-ttu-id="c0b9c-103">За да изтриете Azure AD, уверете се, че:</span><span class="sxs-lookup"><span data-stu-id="c0b9c-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="c0b9c-104">Вие сте глобален администратор в указателя.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="c0b9c-105">НЕ сте влезли с акаунт, който има директорията по подразбиране, като например contoso.onmicrosoft.com, в акаунта за подписано-във, като например admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="c0b9c-106">Премахнете активните приложения в указателя, преди да ги изтриете.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="c0b9c-107">За да премахнете активните приложения, придвижете се до регистрации на приложения и премахнете съществуващите приложения.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="c0b9c-108">Няма активни абонаменти за каквито и да е онлайн услуги на Microsoft, като например Microsoft Azure, Office 365 или Azure AD Premium, свързани в указателя.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="c0b9c-109">Прехвърлете абонаментите си или Ускорете отмяната на активните абонаменти чрез поддръжка на Azure и фактуриране.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="c0b9c-110">Научете повече за това как да отмените абонамента за Office 365 и Azure.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="c0b9c-111">За насоки относно свързването или добавянето на съществуващ абонамент към клиент вижте [свързване или добавяне на абонамент за Azure към вашия клиент на AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="c0b9c-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="c0b9c-112">Няма активни лицензи.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-112">There are no Active license.</span></span> <span data-ttu-id="c0b9c-113">За да премахнете лицензи, вижте [как да премахнете абонамент, за да премахнете лиценза](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="c0b9c-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="c0b9c-114">Няма други активни потребители в директорията освен себе си като глобален администратор при опит за изтриване на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="c0b9c-115">Премахнете всички други активни потребители и всички зависимости в име на домейн по избор в клиента също ще трябва да бъдат премахнати, като например потребители, създадени с admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="c0b9c-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="c0b9c-116">За повече подробности за стъпките относно:</span><span class="sxs-lookup"><span data-stu-id="c0b9c-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="c0b9c-117">Изтрийте "Azure Active Directory" или "Абонамент", вижте [Изтриване на Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="c0b9c-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="c0b9c-118">Премахване на приложения в указателя вижте [Премахване на приложения](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="c0b9c-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
