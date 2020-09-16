---
title: Липсващи фрази от хранилището за изрази на SharePoint online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750440"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="0b732-102">Разрешаване на шифроване с BitLocker с "поднастройване"</span><span class="sxs-lookup"><span data-stu-id="0b732-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="0b732-103">Правилата за защита на крайна точка могат да бъдат използвани за конфигуриране на настройките за шифроване на Boitlocker за устройства с Windows, както е описано в: Windows 10 само (и по-нови версии), за да защитите устройства с помощта на "Настройки"</span><span class="sxs-lookup"><span data-stu-id="0b732-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="0b732-104">Трябва да имате предвид, че много по-нови устройства, на които се изпълнява Windows 10, поддържат автоматично шифроване на BitLocker, което се задейства без прилагане на MDM правилата.</span><span class="sxs-lookup"><span data-stu-id="0b732-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="0b732-105">Това може да се отрази на прилагането на правилата, ако не са конфигурирани настройките по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="0b732-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="0b732-106">Вижте ЧЗВ за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="0b732-106">See FAQ for more detail.</span></span>


<span data-ttu-id="0b732-107">FAQ   Q: кои издания на шифроване на устройства с Windows поддържат използването на правилата за защита на крайна точка?</span><span class="sxs-lookup"><span data-stu-id="0b732-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="0b732-108"> А: настройките в правилата за защита на крайната точка се реализират с помощта на CSP за защитено стартиране.</span><span class="sxs-lookup"><span data-stu-id="0b732-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="0b732-109">Не всички издания или компилации на Windows поддържат CSP за BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="0b732-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="0b732-110">В този момент издания на Windows: Enterprise; Поддържат се обучение, мобилно, мобилно предприятие и професионалист (от компилация 1809 нататък).</span><span class="sxs-lookup"><span data-stu-id="0b732-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="0b732-111">В: Ако дадено устройство вече е шифровано с BitLocker с помощта на настройките по подразбиране за метода на шифроване и якост на шифъра (XTS-AES-128), ще прилага правила с различни настройки автоматично да активира повторно шифроване на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="0b732-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="0b732-112">Отговор: Не.</span><span class="sxs-lookup"><span data-stu-id="0b732-112">A: No.</span></span> <span data-ttu-id="0b732-113">За да приложите новите настройки за шифър, устройството първо трябва да се дешифрира.</span><span class="sxs-lookup"><span data-stu-id="0b732-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="0b732-114">Забележка за устройства, които са записани с автопилот автоматичното шифроване, което ще възникне по време на OOBE, не се задейства, докато не бъде изчислена политиката за настройка, която позволява да се използват настройките за базата на правила, които трябва да бъдат използвани вместо стойностите по подразбиране на операционната система</span><span class="sxs-lookup"><span data-stu-id="0b732-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="0b732-115">В дали дадено устройство е шифровано като резултат от прилагането на правилата за регулиране, то ще се дешифрира, когато се премахне тази политика?</span><span class="sxs-lookup"><span data-stu-id="0b732-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="0b732-116">А: премахването на правилата, свързани с шифроването, не води до дешифриране на устройствата, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="0b732-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="0b732-117">В: защо правилата за съответствие показват, че устройството ми не разполага с "защитено стартиране", но е?</span><span class="sxs-lookup"><span data-stu-id="0b732-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="0b732-118">А: настройката "активирано защитено стартиране" в правилата за съгласуване при прилагане използва клиента за здравна атестация на устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="0b732-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="0b732-119">Този клиент само измерва състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="0b732-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="0b732-120">Така че ако устройството не е било рестартирано, тъй като шифроването на BitLocker е завършило, услугата за клиенти на DHA няма да съобщи за BitLocker като активен.</span><span class="sxs-lookup"><span data-stu-id="0b732-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>