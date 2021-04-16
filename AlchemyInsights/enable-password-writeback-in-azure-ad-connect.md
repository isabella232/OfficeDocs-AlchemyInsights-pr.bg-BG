---
title: Разрешаване на записването на пароли в Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814001"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e989e-102">Разрешаване на записването на пароли в Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e989e-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e989e-103">За да разрешите самостоятелно възстановяване на връщането на паролата, първо разрешете опцията за обратно записване в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e989e-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e989e-104">От вашия сървър на Azure AD Connect изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="e989e-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e989e-105">Влезте в своя сървър на Azure AD Connect и стартирайте съветника за конфигуриране **на Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="e989e-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e989e-106">На страницата **Приветл.** щракнете върху **Конфигуриране**.</span><span class="sxs-lookup"><span data-stu-id="e989e-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e989e-107">На страницата **Допълнителни задачи** изберете Персонализиране на **опциите за синхронизиране** и след това щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="e989e-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e989e-108">На страницата **Свързване към Azure AD** въведете идентификационни данни на глобален администратор за вашия клиент на Azure и след това щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="e989e-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e989e-109">На **страниците Свързване на директории** **и филтриране на домейн/ОЕ** щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="e989e-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e989e-110">На страницата **Незадължителни** функции изберете полето до Възстановяване на парола **и** щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="e989e-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e989e-111">На страницата **Готови за конфигуриране** щракнете върху **Конфигуриране** и изчакайте процесът да завърши.</span><span class="sxs-lookup"><span data-stu-id="e989e-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e989e-112">Когато видите завършването на конфигурацията, щракнете върху **Изход**.</span><span class="sxs-lookup"><span data-stu-id="e989e-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e989e-113">С разрешена парола за записване в Azure AD Connect конфигурирайте Azure AD SSPR за обратно записване.</span><span class="sxs-lookup"><span data-stu-id="e989e-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e989e-114">За да разрешите отписаната парола в SSPR, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="e989e-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e989e-115">Влезте в портала на Azure с помощта на акаунт на глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="e989e-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e989e-116">Потърсете и изберете **Azure Active Directory**, щракнете върху **Нулиране на паролата** и след това **щракнете върху Локална интеграция.**</span><span class="sxs-lookup"><span data-stu-id="e989e-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e989e-117">Задайте опцията за **Пароли за записване обратно в локалния указател?** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="e989e-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e989e-118">Задайте опцията Позволяване **на потребителите да отключват акаунти, без да нулират паролата си?** **на Да**.</span><span class="sxs-lookup"><span data-stu-id="e989e-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e989e-119">Когато сте готови, щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="e989e-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e989e-120">За повече информация вижте Разрешаване на самостоятелно нулиране на паролата за Azure Active Directory в локална [среда.](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="e989e-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e989e-121">Когато администратор нулира паролата на потребител в портала на Azure, ако този потребител е федерирана или се синхронизира хашт с пароли, паролата се записва обратно в локалния.</span><span class="sxs-lookup"><span data-stu-id="e989e-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e989e-122">Тази функционалност изисква лиценз за Azure Premium (P1 или P2) и в момента не се поддържа в портала за администриране на Office.</span><span class="sxs-lookup"><span data-stu-id="e989e-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
