---
title: Автоматично почистване на неактуални устройства в Intune
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
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554740"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="d54a6-102">Автоматично почистване на неактуални устройства в Intune</span><span class="sxs-lookup"><span data-stu-id="d54a6-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="d54a6-103">Intune позволява на администратора да конфигурира интервал от време между 90 и 270 дни, след което остаряла устройства се премахват от услугата.</span><span class="sxs-lookup"><span data-stu-id="d54a6-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="d54a6-104">Тази настройка е организация широк и веднъж активиран влиза в сила веднага.</span><span class="sxs-lookup"><span data-stu-id="d54a6-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="d54a6-105">Всички устройства, които не са проверени в сървъра Intune за период, надвишаващ настройката, се изтриват за постоянно.</span><span class="sxs-lookup"><span data-stu-id="d54a6-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="d54a6-106">**Забележка:** Само MDM обекти на устройство са допустими за това действие за почистване.</span><span class="sxs-lookup"><span data-stu-id="d54a6-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="d54a6-107">EAS само обекти на устройството са изключени.</span><span class="sxs-lookup"><span data-stu-id="d54a6-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="d54a6-108">За допълнителна информация относно това кога дадено устройство отговаря на условията за изтриване въз основа на настройката за почистване на устройството и неговото "състояние":</span><span class="sxs-lookup"><span data-stu-id="d54a6-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="d54a6-109">Настройка: **Изтриване на устройства след последната дата на регистрация: Да (известна стойност (N) в определени дни)**</span><span class="sxs-lookup"><span data-stu-id="d54a6-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="d54a6-110">Въз основа на стойност (N) конфигурирана в настройката, услугата Intune изтрива устройството в определените дни след последната успешно проверка.</span><span class="sxs-lookup"><span data-stu-id="d54a6-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="d54a6-111">Настройка: **Изтриване на устройства след последната дата на регистрация: Не**</span><span class="sxs-lookup"><span data-stu-id="d54a6-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="d54a6-112">180 дни след изтичане на сертификата на устройството и не се подновява, устройството се изтрива.</span><span class="sxs-lookup"><span data-stu-id="d54a6-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="d54a6-113">**Забележка:** И в двата случая устройството трябва да бъде регистрирано успешно в Intune.</span><span class="sxs-lookup"><span data-stu-id="d54a6-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="d54a6-114">Регистрацията възниква по време на първото устройство в проверката на услугата Intune.</span><span class="sxs-lookup"><span data-stu-id="d54a6-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="d54a6-115">Ако устройството се записва успешно Intune, но не се Intune регистриран, устройството се изтрива 270 дни след записване.</span><span class="sxs-lookup"><span data-stu-id="d54a6-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="d54a6-116">(90 дни, за да маркирате устройството като отменено, и след това още 180 дни за изтриване на записа.)</span><span class="sxs-lookup"><span data-stu-id="d54a6-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="d54a6-117">В момента в конзолата intune няма механизъм за установяване на датата на изтичане на сертификата за дадено устройство.</span><span class="sxs-lookup"><span data-stu-id="d54a6-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>