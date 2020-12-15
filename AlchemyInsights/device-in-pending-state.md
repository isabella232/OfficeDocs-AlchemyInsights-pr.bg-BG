---
title: Устройството в очакване на състоянието
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
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/11/2020
ms.locfileid: "49676931"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="877fa-102">Устройството в очакване на състоянието</span><span class="sxs-lookup"><span data-stu-id="877fa-102">Device in pending state</span></span>

<span data-ttu-id="877fa-103">**Предпоставки**</span><span class="sxs-lookup"><span data-stu-id="877fa-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="877fa-104">Ако настройвате регистрации на устройства за първи път, моля, уверете се, че сте прегледали [въвеждането на управление на устройства в Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , което ще ви упъти как да получите устройства под контрола на Azure ad.</span><span class="sxs-lookup"><span data-stu-id="877fa-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="877fa-105">Ако регистрирате устройства в Azure AD директно и ги запишете в [неконфигурирани](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) настройки, трябва да се уверите, че сте конфигурирали предварително и имате първо [лицензите](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .</span><span class="sxs-lookup"><span data-stu-id="877fa-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="877fa-106">Уверете се, че имате разрешение за извършване на операции в Azure AD и локална реклама.</span><span class="sxs-lookup"><span data-stu-id="877fa-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="877fa-107">Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства.</span><span class="sxs-lookup"><span data-stu-id="877fa-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="877fa-108">Освен това, ако настройвате автоматични регистрации във вашия локален указател Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).</span><span class="sxs-lookup"><span data-stu-id="877fa-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="877fa-109">Процесът на регистрация за съединение на Azure AD изисква устройства за включване в корпоративна мрежа.</span><span class="sxs-lookup"><span data-stu-id="877fa-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="877fa-110">Той работи и по VPN, но има някои ограничения за това.</span><span class="sxs-lookup"><span data-stu-id="877fa-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="877fa-111">Чухме клиенти, които се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридната Azure AD при отдалечени работни обстоятелства.</span><span class="sxs-lookup"><span data-stu-id="877fa-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="877fa-112">**Среда за удостоверяване в облака (чрез хеширане при синхронизиране на Azure AD или предавано удостоверяване)**</span><span class="sxs-lookup"><span data-stu-id="877fa-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="877fa-113">Този регистрационен поток е известен също като "съединение за синхронизиране".</span><span class="sxs-lookup"><span data-stu-id="877fa-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="877fa-114">Ето разбивка на това, което се случва по време на процеса на регистриране:</span><span class="sxs-lookup"><span data-stu-id="877fa-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="877fa-115">Windows 10 включва запис за точка на свързване на услугата (SCP), когато потребителят влезе в устройството.</span><span class="sxs-lookup"><span data-stu-id="877fa-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="877fa-116">Устройството първо се опитва да извлече информация за клиента от SCP за клиенти в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="877fa-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="877fa-117">За повече информация вижте [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="877fa-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="877fa-118">Ако то е неуспешно, устройството комуникира с локалния указател Active Directory, за да получи информация за клиента от SCP.</span><span class="sxs-lookup"><span data-stu-id="877fa-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="877fa-119">За да потвърдите SCP, прегледайте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="877fa-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="877fa-120">Препоръчваме ви да разрешавате SCP в Active Directory и да използвате само от страна на клиента SCP за първоначална проверка.</span><span class="sxs-lookup"><span data-stu-id="877fa-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="877fa-121">Windows 10 се опитва да комуникира с Azure AD под системен контекст за удостоверяване срещу Azure AD.</span><span class="sxs-lookup"><span data-stu-id="877fa-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="877fa-122">Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на [скрипта за свързване на регистрационни устройства за проверка на устройството](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="877fa-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="877fa-123">Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локален Active Directory.</span><span class="sxs-lookup"><span data-stu-id="877fa-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="877fa-124">Това изисква наблюдение на домейни за администратора.</span><span class="sxs-lookup"><span data-stu-id="877fa-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="877fa-125">Обект на устройство, който има сертификат, се синхронизира с Azure AD чрез Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="877fa-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="877fa-126">Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но това зависи от конфигурацията на Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="877fa-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="877fa-127">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="877fa-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="877fa-128">На този етап би трябвало да можете да виждате устройството за теми в състояние "**Чакащо**" под "Блейд" на портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="877fa-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="877fa-129">При следващото влизане в Windows 10 регистрацията ще бъде завършена.</span><span class="sxs-lookup"><span data-stu-id="877fa-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="877fa-130">Ако сте на VPN и излизане/влизане прекратява връзката за домейна, можете да активирате регистрацията ръчно.</span><span class="sxs-lookup"><span data-stu-id="877fa-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="877fa-131">За да направите това:</span><span class="sxs-lookup"><span data-stu-id="877fa-131">To do that:</span></span>
    >
    > <span data-ttu-id="877fa-132">Издайте `dsregcmd /join` запитване локално в Админ или отдалечено чрез PSExec на вашия компютър.</span><span class="sxs-lookup"><span data-stu-id="877fa-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="877fa-133">Например: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="877fa-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="877fa-134">За често срещани проблеми с регистрацията на устройства с Azure Active Directory вижте [ЧЗВ](https://docs.microsoft.com/azure/active-directory/devices/faq)за устройството.</span><span class="sxs-lookup"><span data-stu-id="877fa-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
