---
title: Разрешаване на парола нефиксирани в Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560429"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="d1324-102">Разрешаване на парола нефиксирани в Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d1324-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="d1324-103">За да разрешите услугата за самостоятелно нулиране на нефиксирани, първо разрешете опцията нефиксирани в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d1324-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="d1324-104">От вашия сървър на Azure AD Connect изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d1324-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="d1324-105">Влезте в своя сървър на Azure AD Connect и стартирайте съветника за конфигуриране на **AZURE ad Connect** .</span><span class="sxs-lookup"><span data-stu-id="d1324-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="d1324-106">На страницата **добре дошли** щракнете върху **Конфигуриране**.</span><span class="sxs-lookup"><span data-stu-id="d1324-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="d1324-107">На страницата **допълнителни задачи** изберете Персонализиране на **опциите за синхронизиране** и след това щракнете върху **напред**.</span><span class="sxs-lookup"><span data-stu-id="d1324-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="d1324-108">На страницата **Connect to Azure** въведете глобални идентификационни данни на администратор за вашия клиент на Azure и след това щракнете върху **напред**.</span><span class="sxs-lookup"><span data-stu-id="d1324-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="d1324-109">В страниците " **Свързване на указатели** и **домейни/OU** " щракнете върху " **напред**".</span><span class="sxs-lookup"><span data-stu-id="d1324-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="d1324-110">На страницата **опционални функции** изберете квадратчето за отметка до **парола нефиксирани** и щракнете върху **напред**.</span><span class="sxs-lookup"><span data-stu-id="d1324-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="d1324-111">На страницата **готови ли сте да конфигурирате** щракнете върху **Конфигурирай** и изчаквай процесът да завърши.</span><span class="sxs-lookup"><span data-stu-id="d1324-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="d1324-112">Когато видите завършената конфигурация, щракнете върху **изход**.</span><span class="sxs-lookup"><span data-stu-id="d1324-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="d1324-113">С нефиксирани за парола, разрешени в Azure AD Connect, конфигурирайте Azure AD парола за нефиксирани.</span><span class="sxs-lookup"><span data-stu-id="d1324-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="d1324-114">За да разрешите паролата нефиксирани в парола, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="d1324-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="d1324-115">Влезте в портала на Azure чрез акаунт на глобален администратор.</span><span class="sxs-lookup"><span data-stu-id="d1324-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="d1324-116">Потърсете и изберете **Azure Active Directory**, щракнете върху **нулиране на паролата**, след което щракнете върху **локална интеграция**.</span><span class="sxs-lookup"><span data-stu-id="d1324-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="d1324-117">Задаване на опцията за **записване на паролите във вашия локален справочен указател?** **за да**.</span><span class="sxs-lookup"><span data-stu-id="d1324-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="d1324-118">Задаване на опцията за **Разрешаване на потребителите да отключват акаунти без нулиране на паролата си?** **за да**.</span><span class="sxs-lookup"><span data-stu-id="d1324-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="d1324-119">Когато сте готови, щракнете върху **Запиши**.</span><span class="sxs-lookup"><span data-stu-id="d1324-119">When ready, click **Save**.</span></span>

<span data-ttu-id="d1324-120">За повече информация вижте [Разрешаване на услугата за самостоятелно нулиране на паролата за Azure Active Directory нефиксирани към локална среда](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d1324-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="d1324-121">Когато администратор нулира паролата на потребител в портала на Azure, ако този потребител е синхронизиран с външни или хеширани пароли, паролата се записва обратно в локалното.</span><span class="sxs-lookup"><span data-stu-id="d1324-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="d1324-122">Тази функция в момента не се поддържа в портала за администриране на Office.</span><span class="sxs-lookup"><span data-stu-id="d1324-122">This functionality is currently not supported in the Office Admin portal.</span></span>