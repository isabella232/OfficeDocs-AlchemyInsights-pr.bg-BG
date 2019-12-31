---
title: Защита на данните-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908699"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="c3d66-102">Разрешаване на шифроването с InTune</span><span class="sxs-lookup"><span data-stu-id="c3d66-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="c3d66-103">Политика за защита на InTune endpoint може да се използва за конфигуриране на настройките за шифроване на BitLocker за устройства с Windows.</span><span class="sxs-lookup"><span data-stu-id="c3d66-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="c3d66-104">За повече информация вижте [настройките на Windows 10 (и по-нови версии) за защита на устройства с помощта на InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="c3d66-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="c3d66-105">Трябва да знаете, че много по-нови устройства, работещи под Windows 10 поддръжка автоматично шифроване на BitLocker, който се задейства без прилагането на правилата на МДМ.</span><span class="sxs-lookup"><span data-stu-id="c3d66-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="c3d66-106">Това може да повлияе на прилагането на правилата, ако не по подразбиране настройки са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="c3d66-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="c3d66-107">Вижте следните ЧЗВ за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="c3d66-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="c3d66-108">За информация за отстраняване на проблеми със защитеното стартиране вижте [отстраняване на правила за BitLocker в Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="c3d66-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="c3d66-109">**Въпроси**</span><span class="sxs-lookup"><span data-stu-id="c3d66-109">**FAQ**</span></span>

 <span data-ttu-id="c3d66-110">Q: кои издания на Windows поддръжка шифроване на устройства с помощта на правилата за защита на крайни точки?</span><span class="sxs-lookup"><span data-stu-id="c3d66-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="c3d66-111">A: настройките в InTune endpoint защита правила се изпълняват с помощта на [BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)Куу.</span><span class="sxs-lookup"><span data-stu-id="c3d66-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="c3d66-112">Не всички издания или компилации на Windows поддръжка на BitLocker Куу.</span><span class="sxs-lookup"><span data-stu-id="c3d66-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="c3d66-113">По това време се поддържат следните издания на Windows: Enterprise, образование, мобилно устройство, мобилно предприятие и професионалист (компилация 1809 и по-нови).</span><span class="sxs-lookup"><span data-stu-id="c3d66-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="c3d66-114">Q: Ако дадено устройство вече е шифровано с BitLocker с помощта на настройките по подразбиране на OS за метод на шифроване и шифроване сила (XTS-AES-128), ще прилага политика с различни настройки автоматично задейства повторно шифроване на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="c3d66-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="c3d66-115">А: не.</span><span class="sxs-lookup"><span data-stu-id="c3d66-115">A: No.</span></span> <span data-ttu-id="c3d66-116">За да приложите новите настройки за шифроване, устройството трябва първо да бъде дешифрирано.</span><span class="sxs-lookup"><span data-stu-id="c3d66-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="c3d66-117">**Забележка:** За устройства, които се записват с автопилота автоматично шифроване, което ще се случи по време на OOBE не се задейства до InTune правила се оценява, което позволява базирани на правила настройки да се използва на мястото на операционната система по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="c3d66-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="c3d66-118">Въпрос: Ако дадено устройство е шифровано в резултат на прилагането на правилата на InTune, ще бъде ли дешифрирано, когато тази политика бъде премахната?</span><span class="sxs-lookup"><span data-stu-id="c3d66-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="c3d66-119">A: отстраняване на правила, свързани с шифроване не води до дешифрирането на устройствата, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="c3d66-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="c3d66-120">Q: защо InTune правилата за съответствие показват, че устройството ми не е активирана BitLocker, въпреки че е?</span><span class="sxs-lookup"><span data-stu-id="c3d66-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="c3d66-121">A: "BitLocker разрешено" настройка в правилата за съответствие InTune използва Windows Device здравна атестация (DHA) клиент.</span><span class="sxs-lookup"><span data-stu-id="c3d66-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="c3d66-122">Този клиент измерва само състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="c3d66-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="c3d66-123">Така че ако устройството не се рестартира, тъй като шифроването е завършено, услугата за клиент на DHA няма да отчете BitLocker като активен.</span><span class="sxs-lookup"><span data-stu-id="c3d66-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 