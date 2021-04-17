---
title: Ключове за възстановяване на Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820275"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="56090-102">Достъп до клавишите за възстановяване на Bitlocker</span><span class="sxs-lookup"><span data-stu-id="56090-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="56090-103">Когато конфигурирате настройките на Bitlocker Intune Endpoint Protection Policy, е възможно да определите дали информацията за възстановяване на Bitlocker трябва да се съхранява в Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="56090-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="56090-104">Ако тази настройка е конфигурирана, съхранените данни за възстановяване трябва да са видими за администратора на Intune като част от данните за записа на устройството в диска intune Devices по два начина:</span><span class="sxs-lookup"><span data-stu-id="56090-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="56090-105">Устройства – Устройства на Azure AD – > "Устройство" OR Устройства – > Всички устройства – > "Устройство" – > Ключове за възстановяване</span><span class="sxs-lookup"><span data-stu-id="56090-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="56090-106">Като алтернатива, ако има административен достъп до самото устройство, ключът за възстановяване (Парола) може да се види, като изпълните следната команда от команден прозорец с администраторски права:</span><span class="sxs-lookup"><span data-stu-id="56090-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="56090-107">Ако устройството е шифровано преди записването в Intune, ключът за възстановяване може да е свързан с "Акаунт в Microsoft" (MSA), използван за влизане в устройството по време на процеса на OOBE.</span><span class="sxs-lookup"><span data-stu-id="56090-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="56090-108">Ако случаят е такъв, достъпът и влизането с този MSA трябва да показват  https://onedrive.live.com/recoverykey устройствата, за които са съхранени клавишите за възстановяване.</span><span class="sxs-lookup"><span data-stu-id="56090-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="56090-109">Ако устройството е шифровано в резултат на конфигуриране чрез групови правила, базирани на домейни, информацията за възстановяване може да се съхранява в предварителния Active Directory.</span><span class="sxs-lookup"><span data-stu-id="56090-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="56090-110">Ако сте конфигурирали правила за защита на крайни точки, за да съхранявате ключа за възстановяване в Azure Active Directory, но ключът за конкретно устройство не е качен, можете да задействате качването, като завъртате ключа за възстановяване за това устройство от конзолата MEM.</span><span class="sxs-lookup"><span data-stu-id="56090-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="56090-111">За подробности вижте Завъртане на [клавишите за възстановяване на BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span><span class="sxs-lookup"><span data-stu-id="56090-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

