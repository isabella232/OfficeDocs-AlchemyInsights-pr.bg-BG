---
title: Конфигуриране на услугата за предоставяне
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481089"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="4f714-102">Конфигуриране на услугата за предоставяне</span><span class="sxs-lookup"><span data-stu-id="4f714-102">Configuring the Provision service</span></span>

<span data-ttu-id="4f714-103">За автоматизирано осигуряване на потребители за работа Azure AD изисква валидни идентификационни данни, които му позволяват да се свърже с API на уеб услугите на работен ден.</span><span class="sxs-lookup"><span data-stu-id="4f714-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="4f714-104">Освен това, бутонът за проверка на връзката в приложението за осигуряване на работното пространство на AD User също проверява дали може да се свърже с агента за осигуряване на свързване на Azure AD, асоцииран с РЕКЛАМНИя домейн.</span><span class="sxs-lookup"><span data-stu-id="4f714-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="4f714-105">Ако порталът на Azure връща грешка при записване на идентификационните данни, следвайте стъпките по-долу:</span><span class="sxs-lookup"><span data-stu-id="4f714-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="4f714-106">Уверете се, че имате конфигуриран потребителски акаунт за интегриране на работен ден, както е указано в раздела урок [Конфигуриране на потребителя на системата за интегриране в работен ден](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="4f714-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="4f714-107">Уверете се, че услугата за осигуряване на свързване на Azure AD е създадена и се изпълнява на вашия локален сървър на Windows чрез конзолата за управление на услугите.</span><span class="sxs-lookup"><span data-stu-id="4f714-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="4f714-108">Можете също да проверите състоянието на агента в портала на Azure, като щракнете върху бутона Преглед на локалните агенти.</span><span class="sxs-lookup"><span data-stu-id="4f714-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="4f714-109">Уверете се, че въвеждате стойността за поле "потребителско име за работен ден" чрез формата username@workday-Name.</span><span class="sxs-lookup"><span data-stu-id="4f714-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="4f714-110">Ако работният ден – име на клиент липсва, удостоверяването на работния ден е неуспешно.</span><span class="sxs-lookup"><span data-stu-id="4f714-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="4f714-111">Ако конфигурирате интегрирането с клиент за изпълнение на работния ден, обърнете внимание на часовете по график за престой на вашия клиент на работен ден.</span><span class="sxs-lookup"><span data-stu-id="4f714-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="4f714-112">Работният ден е насрочил време за изпълнение на своите наематели през почивните дни (обикновено от петък вечерта към събота сутрин) и неуспешните връзки по време на този прозорец за престои е известен проблем, който автоматично се разрешава веднага щом клиентът за реализиране се върне на линия.</span><span class="sxs-lookup"><span data-stu-id="4f714-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="4f714-113">В редки случаи можете също да видите тази грешка, ако паролата на системата за интегриране е променена поради обновяване на клиента или ако акаунтът е заключен или е изтекъл.</span><span class="sxs-lookup"><span data-stu-id="4f714-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="4f714-114">Моля, проверете състоянието на потребителя на системата за интегриране с администратора на работния си ден.</span><span class="sxs-lookup"><span data-stu-id="4f714-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="4f714-115">За повече информация за конфигурирането на работен ден за автоматизирано осигуряване вижте [урок: Конфигуриране на работен ден за автоматично осигуряване на потребителя](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="4f714-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
