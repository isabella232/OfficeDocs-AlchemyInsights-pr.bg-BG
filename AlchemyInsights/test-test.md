---
title: Липсващи условия от хранилището на онлайн термина на SharePoint
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053502"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="551fd-102">Активиране на шифроването с InTune</span><span class="sxs-lookup"><span data-stu-id="551fd-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="551fd-103">Политиката за защита на InTune endpoint може да се използва за конфигуриране на настройките за шифроване на "Бог" за устройства с Windows, както е описано в: Windows10 (и по-нови) настройки за защита на устройствата, използващи InTune</span><span class="sxs-lookup"><span data-stu-id="551fd-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="551fd-104">Трябва да имате предвид, че много по-нови устройства, работещи под Windows 10 поддръжка автоматично BitLocker шифроване, който се задейства без прилагането на правилата на МДМ.</span><span class="sxs-lookup"><span data-stu-id="551fd-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="551fd-105">Това може да повлияе на прилагането на правилата, ако не настройки по подразбиране са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="551fd-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="551fd-106">Вижте ЧЗВ за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="551fd-106">See FAQ for more detail.</span></span>


<span data-ttu-id="551fd-107">ЧЗВ  Q: кои издания на шифроването на устройства с поддръжка на Windows с помощта на правилата за защита на крайни точки?</span><span class="sxs-lookup"><span data-stu-id="551fd-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="551fd-108"> A: настройките в InTune endpoint защита правила се изпълняват с помощта на BitLocker Куу.</span><span class="sxs-lookup"><span data-stu-id="551fd-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="551fd-109">Не всички издания или компилации на Windows поддръжка на BitLocker Куу. 
     </span><span class="sxs-lookup"><span data-stu-id="551fd-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="551fd-110">По това време изданията на Windows: Enterprise; Образование, мобилен, мобилно предприятие и професионалист (от компилация 1809 нататък) се поддържат.</span><span class="sxs-lookup"><span data-stu-id="551fd-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="551fd-111">Q: Ако дадено устройство вече е шифровано с BitLocker с помощта на настройките по подразбиране на OS за метод на шифроване и шифроване сила (XTS-AES-128) ще прилага политика с различни настройки автоматично задейства повторно шифроване на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="551fd-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="551fd-112">А: не.</span><span class="sxs-lookup"><span data-stu-id="551fd-112">A: No.</span></span> <span data-ttu-id="551fd-113">За да приложите новите настройки за шифроване, устройството трябва първо да бъде дешифрирано.</span><span class="sxs-lookup"><span data-stu-id="551fd-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="551fd-114">Забележка: за устройства, които се записват с автопилота автоматично шифроване, което ще възникне по време на OOBE не се задейства до InTune правила се оценява, което позволява правила базирани настройки да се използва на мястото на операционната система по подразбиране</span><span class="sxs-lookup"><span data-stu-id="551fd-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="551fd-115">Q ако устройството е шифровано в резултат на прилагането на правилата на InTune ще бъде дешифриран, когато тази политика се премахва?</span><span class="sxs-lookup"><span data-stu-id="551fd-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="551fd-116">A: премахване на шифроване, свързани с правилата не води до дешифрирането на устройствата, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="551fd-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="551fd-117">Q: защо InTune правила за съответствие показват, че моето устройство не е "BitLocker разрешено", но това е?</span><span class="sxs-lookup"><span data-stu-id="551fd-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="551fd-118">A: "BitLocker разрешено" настройка в правилата за InTune съответствие използва клиента на Windows устройство здравна атестация (DHA).</span><span class="sxs-lookup"><span data-stu-id="551fd-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="551fd-119">Този клиент измерва само състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="551fd-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="551fd-120">Така че ако устройството не е рестартира, тъй като шифроването е завършило услугата за DHA клиент няма да отчете BitLocker като активен.</span><span class="sxs-lookup"><span data-stu-id="551fd-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>