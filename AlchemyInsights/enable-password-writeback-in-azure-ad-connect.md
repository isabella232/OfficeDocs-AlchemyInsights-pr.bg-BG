---
title: Разрешаване на парола кеш с отслак в Azure AD свързване
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204614"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="1189c-102">Разрешаване на парола кеш с отслак в Azure AD свързване</span><span class="sxs-lookup"><span data-stu-id="1189c-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="1189c-103">За да разрешите самостоятелно парола възстановяване кеш с отсла страна, първо активирайте опцията за отписване в Azure AD свързване.</span><span class="sxs-lookup"><span data-stu-id="1189c-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="1189c-104">От вашия Azure AD свързване сървър изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="1189c-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="1189c-105">Влезте в Azure AD свързване сървър и стартирайте **Azure AD свързване** съветника за конфигуриране.</span><span class="sxs-lookup"><span data-stu-id="1189c-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="1189c-106">На страницата **с приветствие** щракнете върху **Конфигуриране**.</span><span class="sxs-lookup"><span data-stu-id="1189c-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="1189c-107">На страницата **Допълнителни задачи** изберете Персонализиране **на опциите за синхронизация**, след което щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="1189c-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="1189c-108">Свързване **към Azure AD** страница въведете идентификационните данни на глобален администратор за вашия клиент в Azure и след това щракнете върху напред.</span><span class="sxs-lookup"><span data-stu-id="1189c-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="1189c-109">В **свързвате директории** и **домейн/ОЕ** филтриране страници щракнете върху **напред**.</span><span class="sxs-lookup"><span data-stu-id="1189c-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="1189c-110">На страницата **по избор на функции** поставете отметка в квадратчето до Парола **отписване** и щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="1189c-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="1189c-111">На **страницата Готови за конфигуриране** щракнете върху **Конфигуриране** и изчакайте процесът да завърши.</span><span class="sxs-lookup"><span data-stu-id="1189c-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="1189c-112">Когато видите завършването на конфигурацията, щракнете върху **Изход**.</span><span class="sxs-lookup"><span data-stu-id="1189c-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="1189c-113">С парола кеш с отписване разрешено в Azure AD свързване, сега конфигурирайте Azure AD SSPR за отписване.</span><span class="sxs-lookup"><span data-stu-id="1189c-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="1189c-114">За да разрешите парола кеш с отпращане в SSPR, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="1189c-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="1189c-115">Влезте в портала на Azure с помощта на глобален акаунт на администратор.</span><span class="sxs-lookup"><span data-stu-id="1189c-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="1189c-116">Потърсете и изберете **Azure Active Directory**, щракнете върху **Нулиране на паролата**, след което изберете Локално **интегриране**.</span><span class="sxs-lookup"><span data-stu-id="1189c-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="1189c-117">Задаване на опцията за **Запис на пароли за вашия локална директория** да. **Yes**</span><span class="sxs-lookup"><span data-stu-id="1189c-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="1189c-118">Задаване на опцията за **Разрешаване на потребителите да отключват акаунти, без да се нулира паролата си** да . **Yes**</span><span class="sxs-lookup"><span data-stu-id="1189c-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="1189c-119">Когато сте готови, щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="1189c-119">When ready, click **Save**.</span></span>

<span data-ttu-id="1189c-120">За повече информация вижте [Разрешаване Azure Active Directory самостоятелно парола нулиране кеш с обратно в локална среда](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="1189c-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
