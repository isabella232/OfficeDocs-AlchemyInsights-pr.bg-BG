---
title: Влизане в Windows 10 без използване на парола
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830535"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="85656-102">Влизане в Windows 10 без използване на парола</span><span class="sxs-lookup"><span data-stu-id="85656-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="85656-103">За да избегнете въвеждане на парола при стартиране на Windows, ви препоръчваме да използвате една от опциите за защитено влизане в Windows Hello, като например ПИН код, разпознаване на лица или пръстов отпечатък, ако има такива.</span><span class="sxs-lookup"><span data-stu-id="85656-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="85656-104">Ако наистина искате да забраните защитеното влизане, вижте инструкциите "Автоматично влизане в Windows 10" по-долу.</span><span class="sxs-lookup"><span data-stu-id="85656-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="85656-105">**Защитени алтернативи на Windows Hello на паролата за акаунта**</span><span class="sxs-lookup"><span data-stu-id="85656-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="85656-106">Отидете на **Настройки > акаунти > за влизане** (или щракнете [тук](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="85656-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="85656-107">Наличните опции за влизане ще бъдат изброени.</span><span class="sxs-lookup"><span data-stu-id="85656-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="85656-108">Например:</span><span class="sxs-lookup"><span data-stu-id="85656-108">For example:</span></span>

![Опции за влизане.](media/sign-in-options.png)

<span data-ttu-id="85656-110">Щракнете върху или докоснете една от опциите, за да я конфигурирате.</span><span class="sxs-lookup"><span data-stu-id="85656-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="85656-111">Следващия път, когато стартирате или отключите Windows, ще можете да използвате новата опция вместо парола.</span><span class="sxs-lookup"><span data-stu-id="85656-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="85656-112">**Автоматично влизане в Windows 10**</span><span class="sxs-lookup"><span data-stu-id="85656-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="85656-113">**Забележка:** Автоматичното влизане е удобно, но въвежда риск за защитата, особено ако компютърът ви е достъпен от няколко души.</span><span class="sxs-lookup"><span data-stu-id="85656-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="85656-114">Щракнете върху или докоснете **бутона Старт** в лентата на задачите.</span><span class="sxs-lookup"><span data-stu-id="85656-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="85656-115">Въведете **netplwiz и** натиснете клавиша Enter, за да отворите прозореца Потребителски акаунти.</span><span class="sxs-lookup"><span data-stu-id="85656-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="85656-116">В **Потребителски акаунти** щракнете върху акаунта, в който искате да влезете автоматично, когато се стартира Windows.</span><span class="sxs-lookup"><span data-stu-id="85656-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="85656-117">Премахнете отметката от квадратчето "Потребителите трябва да въвеждат потребителско име и парола, за да използват този компютър".</span><span class="sxs-lookup"><span data-stu-id="85656-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Потребителите трябва да въвеждат опция за потребителско име и парола.](media/users-must-enter-username.png)

5. <span data-ttu-id="85656-119">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="85656-119">Click **OK**.</span></span> <span data-ttu-id="85656-120">Ще бъдете помолени да въведете и потвърдите паролата за акаунта, който сте избрали.</span><span class="sxs-lookup"><span data-stu-id="85656-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="85656-121">Щракнете върху **OK,** за да завършите.</span><span class="sxs-lookup"><span data-stu-id="85656-121">Click **OK** to finish.</span></span> <span data-ttu-id="85656-122">Следващия път, когато Windows 10 се стартира, той автоматично ще влиза в акаунта, който сте избрали.</span><span class="sxs-lookup"><span data-stu-id="85656-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
