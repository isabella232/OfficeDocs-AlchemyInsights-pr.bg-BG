---
title: Ключове за възстановяване на BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908804"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="3fcd1-102">Достъп до клавишите за възстановяване на BitLocker</span><span class="sxs-lookup"><span data-stu-id="3fcd1-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="3fcd1-103">При конфигуриране на настройките на BitLocker InTune endpoint Protection правила, е възможно да определите дали информацията за възстановяване на BitLocker трябва да се съхранява в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fcd1-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="3fcd1-104">Ако тази настройка е конфигурирана, съхранените данни за възстановяване трябва да бъдат видими за InTune Admin като част от данните за запис на данни в острието на InTune устройства по два начина:</span><span class="sxs-lookup"><span data-stu-id="3fcd1-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="3fcd1-105">Устройства-Azure AD устройства-> "устройство" или устройства-> всички устройства-> "устройство"-> ключове за възстановяване</span><span class="sxs-lookup"><span data-stu-id="3fcd1-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="3fcd1-106">Алтернативно, ако има администраторски достъп до самото устройство, ключ за възстановяване (Password) може да се види като изпълните следната команда от команден ред с повишени права:</span><span class="sxs-lookup"><span data-stu-id="3fcd1-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="3fcd1-107">Ако устройството е шифровано преди записването в InTune, ключът за възстановяване може да е свързан с "акаунт в Microsoft" (МУИ), използван за влизане в устройството по време на процеса на OOBE.</span><span class="sxs-lookup"><span data-stu-id="3fcd1-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="3fcd1-108">Ако случаят е такъв, достъпът https://onedrive.live.com/recoverykey и влизането с този Муи трябва да показват устройствата, за които са били съхранени ключовете за възстановяване.</span><span class="sxs-lookup"><span data-stu-id="3fcd1-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="3fcd1-109">Ако устройството е шифровано в резултат на конфигурация чрез базирани на домейна групови правила, информацията за възстановяване може да се съхранява в локалната Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3fcd1-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

