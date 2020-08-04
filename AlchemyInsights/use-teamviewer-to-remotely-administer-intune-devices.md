---
title: Използване на TeamViewer за дистанционно администриране на устройства с Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554742"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="9a060-102">Използване на TeamViewer за дистанционно администриране на устройства с Intune</span><span class="sxs-lookup"><span data-stu-id="9a060-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="9a060-103">Устройствата, управлявани от Intune, могат да се прилагат дистанционно с помощта на [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="9a060-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="9a060-104">За администриране на Intune чрез TeamViewer, използвайте следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="9a060-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="9a060-105">Започнете чрез получаване на идентификационни данни от TeamViewer за създаване на TeamViewer конектор на Intune.</span><span class="sxs-lookup"><span data-stu-id="9a060-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="9a060-106">Това позволява на администратора да въвежда идентификационни данни в Потребителския интерфейс на TeamViewer Connector под устройства, еднократна операция за установяване на връзката между Intune и TeamViewer услугата.</span><span class="sxs-lookup"><span data-stu-id="9a060-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="9a060-107">**Част 1: Стартиране на сесия с отдалечено устройство**</span><span class="sxs-lookup"><span data-stu-id="9a060-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="9a060-108">Под **Всички устройства**изберете устройството, с което искате да стартирате отдалечена сесия.</span><span class="sxs-lookup"><span data-stu-id="9a060-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="9a060-109">От **... Още**изберете **Нова сесия за отдалечена помощ**.</span><span class="sxs-lookup"><span data-stu-id="9a060-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="9a060-110">Изберете **Да,** за да потвърдите, че искате да установите отдалечена сесия.</span><span class="sxs-lookup"><span data-stu-id="9a060-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="9a060-111">След като заявката "Иницииране на нова отдалечена сесия" е призната от teamViewer услуга, ще видите опция за **стартиране на отдалечена помощ** под информацията от екрана Преглед (или, Основни) за устройството.</span><span class="sxs-lookup"><span data-stu-id="9a060-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="9a060-112">Изберете **"Вижте още",** за да разгънете екрана и да покажете състоянието на отдалечената помощ.</span><span class="sxs-lookup"><span data-stu-id="9a060-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="9a060-113">Изберете **Стартиране на отдалечена сесия,** за да започнете сесията от страната на администратора.</span><span class="sxs-lookup"><span data-stu-id="9a060-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="9a060-114">Изберете да изтеглите TeamViewer двоичен (Windows) и изберете **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="9a060-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="9a060-115">**Забележка:** Можете да игнорирате всяка страница на уеб браузър, отворена към уеб сайта на TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="9a060-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="9a060-116">Потвърдете искането на teamViewer приложението да прави промени на устройството (само за Windows).</span><span class="sxs-lookup"><span data-stu-id="9a060-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="9a060-117">Приложението TeamViewer се стартира и включва кода на сесията, за да удостоверите връзката с отдалеченото устройство.</span><span class="sxs-lookup"><span data-stu-id="9a060-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="9a060-118">**Част 2: На устройството, което е насочено за отдалечена сесия**</span><span class="sxs-lookup"><span data-stu-id="9a060-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="9a060-119">Отворете портала на фирмата Intune.</span><span class="sxs-lookup"><span data-stu-id="9a060-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="9a060-120">Потърсете флаг за известие: "Вашият ИТ администратор иска контрол на това устройство за сесия за отдалечена помощ" и изберете известието.</span><span class="sxs-lookup"><span data-stu-id="9a060-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="9a060-121">Изберете да изтеглите приложението TeamViewer или да потвърдите изтеглянето на приложението TeamViewer от магазина за приложения и изберете **Изпълнение**.</span><span class="sxs-lookup"><span data-stu-id="9a060-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="9a060-122">**Забележка:** Можете да игнорирате всяка страница на уеб браузър, отворена към уеб сайта на TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="9a060-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="9a060-123">Потвърдете искането на teamViewer приложението да прави промени на устройството (само за Windows).</span><span class="sxs-lookup"><span data-stu-id="9a060-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="9a060-124">Приложението TeamViewer се стартира и включва кода на сесията, за да удостоверите връзката с отдалеченото устройство.</span><span class="sxs-lookup"><span data-stu-id="9a060-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="9a060-125">Изскачащ прозорец пита дали искате да позволите на сесията да започне.</span><span class="sxs-lookup"><span data-stu-id="9a060-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="9a060-126">**Забележка:** Кодовете на сесиите, генерирани от услугата TeamViewer, са само еднократни.</span><span class="sxs-lookup"><span data-stu-id="9a060-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="9a060-127">Ако загубите връзката, трябва:</span><span class="sxs-lookup"><span data-stu-id="9a060-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="9a060-128">Затворете екземпляра на TeamViewer приложението на отдалеченото устройство и на администраторската работна станция.</span><span class="sxs-lookup"><span data-stu-id="9a060-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="9a060-129">Затворете портала на фирмата на отдалеченото устройство.</span><span class="sxs-lookup"><span data-stu-id="9a060-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="9a060-130">Стартиране на нова "Нова отдалечена помощ" от администраторския портал.</span><span class="sxs-lookup"><span data-stu-id="9a060-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="9a060-131">Отворете отново портала на фирмата на отдалеченото устройство, за да получите новото уведомление.</span><span class="sxs-lookup"><span data-stu-id="9a060-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="9a060-132">Изтеглете и отворете приложението TeamViewer както на отдалеченото, така и на администраторската работна станция, както преди.</span><span class="sxs-lookup"><span data-stu-id="9a060-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>