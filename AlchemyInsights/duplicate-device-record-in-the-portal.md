---
title: Дублиране на запис на устройство в портала
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
- "9001495"
- "4386"
ms.openlocfilehash: e32486236a318ae820538cf87c2019e05470211d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47678493"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="ed0cd-102">Дублиране на запис на устройство в портала</span><span class="sxs-lookup"><span data-stu-id="ed0cd-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="ed0cd-103">Може да видите 2 записа за дадено устройство в портала, ако устройството не съобщи правилно състоянието на съвместно управление на сайта на диспечера за конфигуриране.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="ed0cd-104">За да проверите състоянието на съвместно управление на устройство, прегледайте колоната за **Съвместно управление** за устройството в конзолата на диспечера за конфигуриране.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="ed0cd-105">Ако колоната не е видима, можете да я добавите, като щракнете с десния бутон върху някоя от заглавките на колоните и я изберете от списъка.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="ed0cd-106">Съвместно управляваната стойност трябва да бъде **Да**.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="ed0cd-107">Ако стойността е **Не**, отворете аплета за клиента на диспечера за конфигуриране на клиента и проверете свойството **Съвместно управление** в раздела Общи.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="ed0cd-108">Ако стойността е **Разрешено**, това показва проблеми с комуникацията на клиента с точката за управление.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="ed0cd-109">Прегледайте **CcmMessaging.log** на устройството, за да проучите потенциални проблеми при свързването.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="ed0cd-110">Ако стойността е **Забранено** и устройството е записано в настройка, уверете се, че устройството е получило правилата за съвместно управление, като прегледате **CoManagementHandler.log** на устройството.</span><span class="sxs-lookup"><span data-stu-id="ed0cd-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
