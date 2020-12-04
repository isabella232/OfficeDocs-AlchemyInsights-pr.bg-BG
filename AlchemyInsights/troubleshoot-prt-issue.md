---
title: Отстраняване на проблеми с PRT проблема
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573323"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="1773a-102">Отстраняване на проблеми с PRT проблема</span><span class="sxs-lookup"><span data-stu-id="1773a-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="1773a-103">За да завърши удостоверяването на всяко устройство, то трябва да бъде напълно регистрирано и да е в добро състояние и да може да получи първоначален маркер за обновяване (PRT).</span><span class="sxs-lookup"><span data-stu-id="1773a-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="1773a-104">Процесът на регистрация в Azure AD съединение изисква устройства за включване в корпоративна мрежа.</span><span class="sxs-lookup"><span data-stu-id="1773a-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="1773a-105">Той работи и по VPN, но има някои ограничения за това.</span><span class="sxs-lookup"><span data-stu-id="1773a-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="1773a-106">Чухме за потребителите, които се нуждаят от помощ за отстраняване на неизправности при процеса на регистриране на хибридната Azure AD при отдалечени работни обстоятелства.</span><span class="sxs-lookup"><span data-stu-id="1773a-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="1773a-107">Ето разбивка на това, което се случва под капака, по време на процеса на регистрация.</span><span class="sxs-lookup"><span data-stu-id="1773a-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="1773a-108">**Среда за удостоверяване в облака (чрез хеширане при синхронизиране на Azure AD или предавано удостоверяване)**</span><span class="sxs-lookup"><span data-stu-id="1773a-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="1773a-109">Този регистрационен поток е известен също като "съединение за синхронизиране".</span><span class="sxs-lookup"><span data-stu-id="1773a-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="1773a-110">Windows 10 открие SCP запис при влизане на потребителя в устройството.</span><span class="sxs-lookup"><span data-stu-id="1773a-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="1773a-111">Устройството първо се опитва да извлече информация за клиента от SCP за клиенти в системния регистър [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="1773a-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="1773a-112">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="1773a-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="1773a-113">Ако то е неуспешно, устройството комуникира с локалния указател Active Directory (AD), за да получи информация за клиента от точка на свързване на услугата (SCP).</span><span class="sxs-lookup"><span data-stu-id="1773a-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="1773a-114">За да потвърдите SCP, вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="1773a-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="1773a-115">Препоръчваме ви да разрешавате SCP в ОБЯВата и да използвате само от страна на клиента SCP за първоначална проверка.</span><span class="sxs-lookup"><span data-stu-id="1773a-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="1773a-116">Windows 10 се опитва да комуникира с Azure AD под системен контекст за удостоверяване срещу Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1773a-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="1773a-117">Можете да проверите дали устройството има достъп до ресурсите на Microsoft под системния акаунт с помощта на скрипта за свързване на регистрационни устройства за проверка на устройството.</span><span class="sxs-lookup"><span data-stu-id="1773a-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="1773a-118">Windows 10 генерира самоподписан сертификат и го съхранява под обекта на компютъра в локалната реклама.</span><span class="sxs-lookup"><span data-stu-id="1773a-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="1773a-119">Това изисква наблюдение на домейни за администратора.</span><span class="sxs-lookup"><span data-stu-id="1773a-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="1773a-120">Обект на устройство, който има сертификат, се синхронизира с Azure AD чрез Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1773a-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="1773a-121">Цикълът на синхронизиране е на всеки 30 минути по подразбиране, но това зависи от конфигурацията на Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="1773a-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="1773a-122">За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="1773a-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="1773a-123">На този етап би трябвало да можете да виждате устройството за теми в състояние "Чакащо" под "Блейд" на портала на Azure.</span><span class="sxs-lookup"><span data-stu-id="1773a-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="1773a-124">При следващото влизане в Windows 10 регистрацията ще бъде завършена.</span><span class="sxs-lookup"><span data-stu-id="1773a-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="1773a-125">Ако сте в VPN и процесът на излизане при влизане приключи със свързването на домейна, можете да активирате регистрацията ръчно:</span><span class="sxs-lookup"><span data-stu-id="1773a-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="1773a-126">Издайте на dsregcmd/JOIN локално в Админ подкана или отдалечено чрез PSExec на вашия компютър.</span><span class="sxs-lookup"><span data-stu-id="1773a-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="1773a-127">Например PsExec-s \\ win10client01 CMD, dsregcmd/JOIN</span><span class="sxs-lookup"><span data-stu-id="1773a-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="1773a-128">За повече информация относно хибридните проблеми при съединението вижте [отстраняване на](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)проблеми с устройства.</span><span class="sxs-lookup"><span data-stu-id="1773a-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
