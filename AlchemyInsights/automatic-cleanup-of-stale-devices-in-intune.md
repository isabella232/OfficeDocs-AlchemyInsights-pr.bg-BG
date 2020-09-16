---
title: Автоматично почистване на изхабени устройства в съзвучие
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715010"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="9ed2f-102">Автоматично почистване на изхабени устройства в съзвучие</span><span class="sxs-lookup"><span data-stu-id="9ed2f-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="9ed2f-103">Тази настройка позволява на администратора да конфигурира времеви интервал между 90 и 270 дни, след което се премахват остарели устройства от услугата.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="9ed2f-104">Тази настройка представлява широка организация и веднъж активирана веднага влиза в сила.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="9ed2f-105">Всички устройства, които не са отметнати в сървъра за настройка за период, надвишаващ настройката, се изтриват окончателно.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="9ed2f-106">**Забележка** Само обекти на MDM устройства отговарят на условията за това действие за почистване.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="9ed2f-107">Изключват се само обектите на устройството.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="9ed2f-108">За допълнителна информация относно това кога устройството става допустимо за изтриване на базата на настройката за почистване на устройството и неговата "държава":</span><span class="sxs-lookup"><span data-stu-id="9ed2f-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="9ed2f-109">Настройка: **Изтриване на устройства след последната дата за вкарване: да (някои стойности (N) в указаните дни)**</span><span class="sxs-lookup"><span data-stu-id="9ed2f-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="9ed2f-110">На базата на стойност (N), конфигурирана в настройката, услугата настройка изтрива устройството в определените дни, след като последно е извършвал успешно проверки.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="9ed2f-111">Настройка:  **Изтриване на устройства след последната дата за вкарване: не**</span><span class="sxs-lookup"><span data-stu-id="9ed2f-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="9ed2f-112">180 дни, след като сертификатът за устройството изтече и не бъде подновен, устройството се изтрива.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="9ed2f-113">**Забележка** И в двата случая устройството трябва да бъде успешно регистрирано.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="9ed2f-114">Регистрирането възниква по време на първото устройство, което вкарва в услугата за настройване.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="9ed2f-115">Ако дадено устройство се записва успешно за да се настрои, но не стане регистрирано, устройството се изтрива 270 дни след записването.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="9ed2f-116">(90 дни, за да маркирате устройството като анулирано и след това още 180 дни, за да изтриете записа.)</span><span class="sxs-lookup"><span data-stu-id="9ed2f-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="9ed2f-117">В момента не съществува механизъм в конзолата за въвеждане, за да се установи срокът на валидност на сертификата за устройството за дадено устройство.</span><span class="sxs-lookup"><span data-stu-id="9ed2f-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>