---
title: Термини, които липсват от sharePoint Online хранилището на изрази
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766842"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="eaf70-102">Разрешаване на шифроването на Bitlocker с Intune</span><span class="sxs-lookup"><span data-stu-id="eaf70-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="eaf70-103">Intune endpoint Protection Правила може да се използва за конфигуриране на настройките за шифроване Boitlocker за устройства с Windows, както е описано в : Windows10 (и по-нови) настройки за защита на устройства с помощта на Intune</span><span class="sxs-lookup"><span data-stu-id="eaf70-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="eaf70-104">Трябва да знаете, че много по-нови устройства, работещи с Windows 10, поддържат автоматично шифроване на защитеното стартиране, което се задейства без прилагането на MDM политика.</span><span class="sxs-lookup"><span data-stu-id="eaf70-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="eaf70-105">Това може да повлияе на прилагането на правилата, ако настройките по подразбиране са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="eaf70-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="eaf70-106">Вижте Често задавани въпроси за повече подробности.</span><span class="sxs-lookup"><span data-stu-id="eaf70-106">See FAQ for more detail.</span></span>


<span data-ttu-id="eaf70-107">Често  задавани въпроси: Кои издания на Windows поддържат шифроване на устройства с помощта на правилата за защита на крайни точки?</span><span class="sxs-lookup"><span data-stu-id="eaf70-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="eaf70-108"> A: Настройките в Intune endpoint protection правила се изпълняват с помощта на Bitlocker CSP.</span><span class="sxs-lookup"><span data-stu-id="eaf70-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="eaf70-109">Не всички издания, нито изгражда Windows поддържа Bitlocker CSP. 
     </span><span class="sxs-lookup"><span data-stu-id="eaf70-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="eaf70-110">В този момент Windows издания: Enterprise; Образование, мобилна, мобилна enterprise и професионална (от компилация 1809 нататък) се поддържат.</span><span class="sxs-lookup"><span data-stu-id="eaf70-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="eaf70-111">Q: Ако дадено устройство вече е шифровано с Bitlocker, използвайки настройките по подразбиране на операционната система за шифроване метод и шифър (XTS-AES-128) ще прилага политика с различни настройки автоматично задейства повторно криптиране на устройството с новите настройки?</span><span class="sxs-lookup"><span data-stu-id="eaf70-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="eaf70-112">О: Не.</span><span class="sxs-lookup"><span data-stu-id="eaf70-112">A: No.</span></span> <span data-ttu-id="eaf70-113">За да приложите новите настройки за шифроване, първо трябва да се дешифрира устройството.</span><span class="sxs-lookup"><span data-stu-id="eaf70-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="eaf70-114">Забележка: За устройства, които са записани с автопилот автоматично шифроване, което ще се появи по време на OOBE не се задейства, докато Intune правила се оценява което позволява базирани на правила настройки те се използват вместо по подразбиране на операционната система</span><span class="sxs-lookup"><span data-stu-id="eaf70-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="eaf70-115">Q Ако устройството е шифровано в резултат на прилагането на intune политика ще бъде дешифрирано, когато тази политика се премахва?</span><span class="sxs-lookup"><span data-stu-id="eaf70-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="eaf70-116">A: Премахване на правилата, свързани с шифроване не води до дешифриране на устройства, които са конфигурирани.</span><span class="sxs-lookup"><span data-stu-id="eaf70-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="eaf70-117">В: Защо intune Compliance политика показва, че устройството ми няма "Bitlocker разрешено", но е?</span><span class="sxs-lookup"><span data-stu-id="eaf70-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="eaf70-118">A: Настройката "Bitlocker разрешено" в intune съответствие политика използва клиента на Windows устройство изправност (DHA).</span><span class="sxs-lookup"><span data-stu-id="eaf70-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="eaf70-119">Този клиент измерва само състоянието на устройството по време на зареждане.</span><span class="sxs-lookup"><span data-stu-id="eaf70-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="eaf70-120">Така че ако устройството не е рестартирано, тъй като bitlocker шифроването завърши, клиентската услуга DHA няма да отчете bitlocker като активен.</span><span class="sxs-lookup"><span data-stu-id="eaf70-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>