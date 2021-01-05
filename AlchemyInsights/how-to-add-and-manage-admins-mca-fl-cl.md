---
title: Как да добавяте и управлявате администратори
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755428"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="26156-102">Как да добавяте и управлявате администратори</span><span class="sxs-lookup"><span data-stu-id="26156-102">How to add and manage admins</span></span>

<span data-ttu-id="26156-103">Въз основа на вашето описание на проблема намерихме решение за вас.</span><span class="sxs-lookup"><span data-stu-id="26156-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="26156-104">Повечето клиенти могат сами да решат проблема си, след като са следвали нашата документация.</span><span class="sxs-lookup"><span data-stu-id="26156-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="26156-105">За да управлявате своя акаунт за фактуриране за споразумение с клиенти на Microsoft (MCA), можете да използвате различни роли с желаното ниво на достъп.</span><span class="sxs-lookup"><span data-stu-id="26156-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="26156-106">Тези роли са допълнение към вградените роли на Azure услуги, които ви помагат да управлявате ресурсите си.</span><span class="sxs-lookup"><span data-stu-id="26156-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="26156-107">**За да добавите роли на плащане в портала на Azure:**</span><span class="sxs-lookup"><span data-stu-id="26156-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="26156-108">Влезте в портала на [Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="26156-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="26156-109">Потърсете *управление на разходите + плащане*.</span><span class="sxs-lookup"><span data-stu-id="26156-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="26156-110">Изберете контрол на достъпа (IAM) в обхват, като например акаунт за фактуриране, профил за фактуриране или секция за фактура, където искате да дадете достъп.</span><span class="sxs-lookup"><span data-stu-id="26156-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="26156-111">Страницата за контрол на достъпа (IAM) изброява потребителите и групите, на които е присвоена всяка роля за този обхват.</span><span class="sxs-lookup"><span data-stu-id="26156-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="26156-112">За да дадете достъп на потребител, изберете **Добави** от горния край на страницата.</span><span class="sxs-lookup"><span data-stu-id="26156-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="26156-113">В падащия списък *роля* изберете роля.</span><span class="sxs-lookup"><span data-stu-id="26156-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="26156-114">Въведете имейл адреса на потребителя, на когото искате да дадете достъп.</span><span class="sxs-lookup"><span data-stu-id="26156-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="26156-115">Изберете **Запиши** , за да присвоите ролята.</span><span class="sxs-lookup"><span data-stu-id="26156-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="26156-116">За да премахнете достъпа за потребител, изберете потребителя с възложената роля, която искате да премахнете.</span><span class="sxs-lookup"><span data-stu-id="26156-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="26156-117">Изберете **Премахни**.</span><span class="sxs-lookup"><span data-stu-id="26156-117">Select **Remove**.</span></span>

<span data-ttu-id="26156-118">**Препоръчителни документи**</span><span class="sxs-lookup"><span data-stu-id="26156-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="26156-119">Дефиниции на роли на плащане</span><span class="sxs-lookup"><span data-stu-id="26156-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="26156-120">Роли и задачи за акаунт за фактуриране</span><span class="sxs-lookup"><span data-stu-id="26156-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="26156-121">Първи стъпки с вашия МСА акаунт за фактуриране</span><span class="sxs-lookup"><span data-stu-id="26156-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="26156-122">Проверяване на достъпа до клиентско споразумение на Microsoft</span><span class="sxs-lookup"><span data-stu-id="26156-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
