---
title: DataProtection
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731228"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="190cc-102">Разрешаване на шифроване с BitLocker с "поднастройване"</span><span class="sxs-lookup"><span data-stu-id="190cc-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="190cc-103">Правилата за защита на крайна точка могат да се използват за конфигуриране на настройките за шифроване на BitLocker за устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="190cc-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="190cc-104">За повече информация вижте [Настройки на Windows 10 (и по-нови версии), за да защитите устройства, използващи настройка](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="190cc-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="190cc-105">Трябва да знаете, че много по-нови устройства, на които се изпълнява Windows 10, поддържат автоматично шифроване на BitLocker, което се задейства без прилагане на MDM правилата.</span><span class="sxs-lookup"><span data-stu-id="190cc-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="190cc-106">Това може да се отрази на прилагането на правилата, ако са конфигурирани настройки, които не са по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="190cc-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="190cc-107">Вижте следните ЧЗВ за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="190cc-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="190cc-108">За информация относно отстраняването на проблеми с BitLocker вижте Отстраняване на проблеми [с правилата за BitLocker в Microsoft](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="190cc-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="190cc-109">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="190cc-109">**FAQ**</span></span>

 <span data-ttu-id="190cc-110">В: кои издания на шифроване на устройства с Windows поддържат използването на правилата за защита на крайна точка?</span><span class="sxs-lookup"><span data-stu-id="190cc-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="190cc-111">А: настройките в правилата за защита на крайната точка се реализират с помощта на [CSP за защитено стартиране](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="190cc-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="190cc-112">Не всички издания или компилации на Windows поддържат CSP за BitLocker.</span><span class="sxs-lookup"><span data-stu-id="190cc-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="190cc-113">Към този момент се поддържат следните издания на Windows: Enterprise, Education, Mobile, Mobile Enterprise и Professional (компилация 1809 и по-нова версия).</span><span class="sxs-lookup"><span data-stu-id="190cc-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="190cc-114">В: Ако дадено устройство вече е шифровано с BitLocker с помощта на настройките по подразбиране на операционната система за метод на шифроване и якост на шифъра (XTS-AES-128), ще прилагате правила с различни настройки автоматично ще задействате повторно шифроване на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="190cc-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="190cc-115">Отговор: Не.</span><span class="sxs-lookup"><span data-stu-id="190cc-115">A: No.</span></span> <span data-ttu-id="190cc-116">За да приложите новите настройки за шифър, дискът първо трябва да бъде дешифриран.</span><span class="sxs-lookup"><span data-stu-id="190cc-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="190cc-117">**Забележка:** За устройства, които са записани с автопилот, автоматичното шифроване, което ще възникне по време на OOBE, не се активира, докато не бъде изчислена правилата за настройка, което позволява да се използват настройките, базирани на правила, за да бъдат използвани вместо OS по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="190cc-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="190cc-118">В: Ако дадено устройство е шифровано като резултат от прилагането на правилата за регулиране, то ще се дешифрира ли, когато се премахне тази политика?</span><span class="sxs-lookup"><span data-stu-id="190cc-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="190cc-119">А: премахването на свързаните с шифроването правила не води до дешифриране на устройствата, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="190cc-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="190cc-120">В: защо правилата за съответствие показват, че на моето устройство не е активирано BitLocker, въпреки че е?</span><span class="sxs-lookup"><span data-stu-id="190cc-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="190cc-121">А: настройката "активирано защитено стартиране" в правилата за спазване на изискванията използва клиента за удостоверяване на устройства с Windows Health (DHA).</span><span class="sxs-lookup"><span data-stu-id="190cc-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="190cc-122">Този клиент само измерва състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="190cc-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="190cc-123">И така, ако устройството не е било рестартирано, тъй като шифроването на BitLocker е било завършено, услугата за клиенти на DHA няма да съобщи за BitLocker като активен.</span><span class="sxs-lookup"><span data-stu-id="190cc-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 