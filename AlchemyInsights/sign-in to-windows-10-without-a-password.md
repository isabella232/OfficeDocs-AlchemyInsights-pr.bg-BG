---
title: Влизане в Windows 10 без използване на парола
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
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719942"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="1575a-102">Влизане в Windows 10 без използване на парола</span><span class="sxs-lookup"><span data-stu-id="1575a-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="1575a-103">За да не се налага да въвеждате парола при стартиране на Windows, ви препоръчваме да използвате една от опциите за влизане в Windows Hello, като например ПИН, разпознаване на лица или пръстови отпечатъци, ако има такива.</span><span class="sxs-lookup"><span data-stu-id="1575a-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="1575a-104">Ако наистина искате да забраните защитеното влизане, вижте инструкциите "автоматично влизане в Windows 10" по-долу.</span><span class="sxs-lookup"><span data-stu-id="1575a-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="1575a-105">**Защитен Windows Hello алтернативи за паролата на акаунта**</span><span class="sxs-lookup"><span data-stu-id="1575a-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="1575a-106">Отидете на **настройки, за > акаунти > опции за влизане** (или щракнете [тук](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="1575a-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="1575a-107">Ще бъдат показани наличните опции за влизане.</span><span class="sxs-lookup"><span data-stu-id="1575a-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="1575a-108">Например:</span><span class="sxs-lookup"><span data-stu-id="1575a-108">For example:</span></span>

![Опции за влизане.](media/sign-in-options.png)

<span data-ttu-id="1575a-110">Щракнете върху или докоснете една от опциите, за да я конфигурирате.</span><span class="sxs-lookup"><span data-stu-id="1575a-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="1575a-111">Следващия път, когато стартирате или отключите Windows, ще можете да използвате новата опция вместо парола.</span><span class="sxs-lookup"><span data-stu-id="1575a-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="1575a-112">**Автоматично влизане в Windows 10**</span><span class="sxs-lookup"><span data-stu-id="1575a-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="1575a-113">**Забележка**: автоматичното влизане е удобно, но въвежда риск за защитата, особено ако компютърът ви е достъпен от много хора.</span><span class="sxs-lookup"><span data-stu-id="1575a-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="1575a-114">Щракнете върху или докоснете бутона **Старт** в лентата на задачите.</span><span class="sxs-lookup"><span data-stu-id="1575a-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="1575a-115">Въведете **netplwiz** и натиснете клавиша ENTER, за да отворите прозореца потребителски акаунти.</span><span class="sxs-lookup"><span data-stu-id="1575a-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="1575a-116">В **потребителски акаунти**щракнете върху акаунта, в който искате да влизате автоматично при стартиране на Windows.</span><span class="sxs-lookup"><span data-stu-id="1575a-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="1575a-117">Изчистете отметката от квадратчето "потребители трябва да въведат потребителско име и парола, за да използват този компютър".</span><span class="sxs-lookup"><span data-stu-id="1575a-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Потребителят трябва да въведе опция за потребителско име и парола.](media/users-must-enter-username.png)

5. <span data-ttu-id="1575a-119">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="1575a-119">Click **OK**.</span></span> <span data-ttu-id="1575a-120">Ще бъдете подканени да въведете и да потвърдите паролата за акаунта, който сте избрали.</span><span class="sxs-lookup"><span data-stu-id="1575a-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="1575a-121">Щракнете върху **OK** , за да завършите.</span><span class="sxs-lookup"><span data-stu-id="1575a-121">Click **OK** to finish.</span></span> <span data-ttu-id="1575a-122">Следващия път, когато Windows 10 се стартира, той автоматично ще влезе в акаунта, който сте избрали.</span><span class="sxs-lookup"><span data-stu-id="1575a-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
