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
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768806"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="245c6-102">Разрешаване на шифроване с BitLocker с "поднастройване"</span><span class="sxs-lookup"><span data-stu-id="245c6-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="245c6-103">Правилата за защита на крайна точка могат да се използват за конфигуриране на настройките за шифроване на BitLocker за устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="245c6-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="245c6-104">За повече информация вижте [Настройки на Windows 10 (и по-нови версии), за да защитите устройства, използващи настройка](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="245c6-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="245c6-105">Трябва да знаете, че много по-нови устройства, на които се изпълнява Windows 10, поддържат автоматично шифроване на BitLocker, което се задейства без прилагане на MDM правилата.</span><span class="sxs-lookup"><span data-stu-id="245c6-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="245c6-106">Това може да се отрази на прилагането на правилата, ако са конфигурирани настройки, които не са по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="245c6-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="245c6-107">Вижте следните ЧЗВ за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="245c6-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="245c6-108">За информация относно отстраняването на проблеми с BitLocker вижте Отстраняване на проблеми [с правилата за BitLocker в Microsoft](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="245c6-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="245c6-109">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="245c6-109">**FAQ**</span></span>

<span data-ttu-id="245c6-110">В: кои издания на шифроване на устройства с Windows поддържат използването на правилата за защита на крайна точка?</span><span class="sxs-lookup"><span data-stu-id="245c6-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="245c6-111">А: настройките в правилата за защита на крайната точка се реализират с помощта на [CSP за защитено стартиране](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="245c6-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="245c6-112">Не всички издания или компилации на Windows поддържат CSP за BitLocker.</span><span class="sxs-lookup"><span data-stu-id="245c6-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="245c6-113">В: как да се разреши BitLocker на устройства, без да се изисква взаимодействие с крайния потребител?</span><span class="sxs-lookup"><span data-stu-id="245c6-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="245c6-114">А: дотолкова, доколкото необходимите предварителни условия са изпълнени, е възможно да се разреши защитено шифроване "безшумен" чрез настройване.</span><span class="sxs-lookup"><span data-stu-id="245c6-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="245c6-115">Вижте подробните данни за изискванията към устройството и примерните настройки на правилата, за да разрешите шифроването на безшумен режим в следния документ: [мълчаливо Активирайте шифроването с BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="245c6-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="245c6-116">В: Ако дадено устройство вече е шифровано с BitLocker с помощта на настройките по подразбиране на операционната система за метод на шифроване и якост на шифъра (XTS-AES-128), ще прилагате правила с различни настройки автоматично ще задействате повторно шифроване на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="245c6-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="245c6-117">Отговор: Не.</span><span class="sxs-lookup"><span data-stu-id="245c6-117">A: No.</span></span> <span data-ttu-id="245c6-118">За да приложите новите настройки за шифър, дискът първо трябва да бъде дешифриран.</span><span class="sxs-lookup"><span data-stu-id="245c6-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="245c6-119">**Забележка:** За устройства, които са записани с автопилот, автоматичното шифроване, което ще възникне по време на OOBE, не се активира, докато не бъде изчислена правилата за настройка, което позволява да се използват настройките, базирани на правила, за да бъдат използвани вместо OS по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="245c6-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="245c6-120">В: Ако дадено устройство е шифровано като резултат от прилагането на правилата за регулиране, то ще се дешифрира ли, когато се премахне тази политика?</span><span class="sxs-lookup"><span data-stu-id="245c6-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="245c6-121">А: премахването на свързаните с шифроването правила не води до дешифриране на устройствата, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="245c6-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="245c6-122">В: защо правилата за съответствие показват, че на моето устройство не е активирано BitLocker, въпреки че е?</span><span class="sxs-lookup"><span data-stu-id="245c6-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="245c6-123">А: настройката "активирано защитено стартиране" в правилата за спазване на изискванията използва клиента за удостоверяване на устройства с Windows Health (DHA).</span><span class="sxs-lookup"><span data-stu-id="245c6-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="245c6-124">Този клиент само измерва състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="245c6-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="245c6-125">И така, ако устройството не е било рестартирано, тъй като шифроването на BitLocker е било завършено, услугата за клиенти на DHA няма да съобщи за BitLocker като активен.</span><span class="sxs-lookup"><span data-stu-id="245c6-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 