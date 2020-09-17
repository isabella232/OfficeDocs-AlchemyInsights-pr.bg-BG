---
title: Използвайте опцията за отключване на пръстови отпечатъци в Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795233"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="8f228-102">Използвайте опцията за отключване на пръстови отпечатъци в Windows 10</span><span class="sxs-lookup"><span data-stu-id="8f228-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="8f228-103">**Разрешаване на Windows Hello пръстови отпечатъци**</span><span class="sxs-lookup"><span data-stu-id="8f228-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="8f228-104">За да отключите Windows 10 с помощта на пръстови отпечатъци, трябва да настроите Windows Hello fingerprint чрез добавяне (оставяне на Windows да се научи да разпознава) поне един пръст.</span><span class="sxs-lookup"><span data-stu-id="8f228-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="8f228-105">Отидете на **настройки, за > акаунти > опции за влизане** (или щракнете [тук](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="8f228-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8f228-106">Ще бъдат показани наличните опции за влизане.</span><span class="sxs-lookup"><span data-stu-id="8f228-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="8f228-107">Например:</span><span class="sxs-lookup"><span data-stu-id="8f228-107">For example:</span></span>

    ![Опции за влизане.](media/sign-in-options.png)

2. <span data-ttu-id="8f228-109">Щракнете върху или докоснете **Windows Hello пръстови отпечатъци**, след което щракнете върху **Настройка**.</span><span class="sxs-lookup"><span data-stu-id="8f228-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="8f228-110">В прозореца на инсталиращата програма на Windows Hello щракнете върху **Първи стъпки**.</span><span class="sxs-lookup"><span data-stu-id="8f228-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="8f228-111">Сензорът за пръстови отпечатъци ще бъде активиран и ще бъдете помолени да поставите пръст върху сензора:</span><span class="sxs-lookup"><span data-stu-id="8f228-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Сензор за пръстови отпечатъци.](media/fingerprint-sensor.png)

3. <span data-ttu-id="8f228-113">Следвайте инструкциите, които ще ви накарат да сканирате многократно пръста си.</span><span class="sxs-lookup"><span data-stu-id="8f228-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="8f228-114">Когато това приключи, ще имате възможност да добавите други пръсти, които може да поискате да използвате за влизане.</span><span class="sxs-lookup"><span data-stu-id="8f228-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="8f228-115">Следващия път, когато влезете в Windows 10, ще имате възможност да използвате пръстови отпечатъци, за да го направите.</span><span class="sxs-lookup"><span data-stu-id="8f228-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="8f228-116">**"Windows Hello пръстови отпечатъци" не е наличен като опция за влизане**</span><span class="sxs-lookup"><span data-stu-id="8f228-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="8f228-117">Ако "Windows Hello fingerprint" не се показва като опция в " **Опции за влизане**", това означава, че Windows не е наясно с четеца/скенера за пръстови отпечатъци, прикачени към компютъра или че правилата на системата предотвратяват употребата му (ако НАПРИМЕР вашият компютър се управлява от работното ви място).</span><span class="sxs-lookup"><span data-stu-id="8f228-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="8f228-118">За отстраняване на неизправности:</span><span class="sxs-lookup"><span data-stu-id="8f228-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="8f228-119">Изберете бутона " **Старт** " в лентата на задачите и потърсете **Диспечер на устройствата**.</span><span class="sxs-lookup"><span data-stu-id="8f228-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="8f228-120">Щракнете върху или докоснете, за да отворите **диспечера на устройствата**.</span><span class="sxs-lookup"><span data-stu-id="8f228-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="8f228-121">В диспечера на устройствата разгънете биометрични устройства чрез щракване върху нейната Шеврон.</span><span class="sxs-lookup"><span data-stu-id="8f228-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Биометрични устройства.](media/biometric-devices.png)

4. <span data-ttu-id="8f228-123">Скенерът на пръстови отпечатъци трябва да бъде показан като биометрична устройство, като например Synaptics WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="8f228-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Биометрични устройства.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="8f228-125">Ако скенерът ви за пръстови отпечатъци не е показан и скенерът е вграден в КОМПЮТЪРА ви, отидете на уеб сайта на производителя на КОМПЮТЪРА.</span><span class="sxs-lookup"><span data-stu-id="8f228-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="8f228-126">В секцията техническа поддръжка за модела на КОМПЮТЪРА Потърсете драйвер за Windows 10 за скенер, който можете да инсталирате.</span><span class="sxs-lookup"><span data-stu-id="8f228-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="8f228-127">Ако скенерът е отделен от КОМПЮТЪРА (прикачен чрез USB), отидете на уеб сайта на производителя на скенера, за да намерите и инсталирате софтуера на драйвера за устройство с Windows 10 за модела на скенера, който имате.</span><span class="sxs-lookup"><span data-stu-id="8f228-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
