---
title: Синхронизиране на пароли
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480989"
---
# <a name="password-synchronization"></a><span data-ttu-id="c9e06-102">Синхронизиране на пароли</span><span class="sxs-lookup"><span data-stu-id="c9e06-102">Password synchronization</span></span>

<span data-ttu-id="c9e06-103">**Синхронизирането на хеширане с парола изобщо не работи**</span><span class="sxs-lookup"><span data-stu-id="c9e06-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="c9e06-104">Някои често срещани проблеми, при които се сблъскват потребителите при синхронизиране на хеширане с парола, са:</span><span class="sxs-lookup"><span data-stu-id="c9e06-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="c9e06-105">Акаунтът за Active Directory, използван от Azure AD Connect за комуникиране с локален указател Active Directory, не се разрешава за **повтарящи се промени в справочните указатели** и за **реплициране на всички** разрешения, които са необходими за синхронизиране на парола – трябва да коригирате това, като предоставите тези разрешения на акаунта на Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9e06-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="c9e06-106">Синхронизацията на хеширане с парола е забранена, след като администраторът е променил метода на потребителя Sign-In от **Синхронизиране на парола** с друга опция, като например **ФЕДЕРАЦИЯТА с AD FS** в съветника за свързване на Azure ad – можете да го поправите чрез повторно разрешаване на функцията за **Синхронизиране на хеширане с парола**</span><span class="sxs-lookup"><span data-stu-id="c9e06-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="c9e06-107">Проблем със свързването с локален Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9e06-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="c9e06-108">Например някои домейнови контролери не са достъпни чрез Azure AD Connect или [изискваните портове](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) са блокирани от защитната стена – трябва да коригирате това, като се уверите, че свързването между сървъра на Azure ad Connect и локалната Active Directory работи правилно.</span><span class="sxs-lookup"><span data-stu-id="c9e06-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="c9e06-109">Сървър на Azure AD Connect, който в момента е в режим на спиране, което ще доведе до това, че сървърът не е в състояние да използва Хеширането на парола – за да отстраните проблема, следвайте стъпките, описани в раздела отстраняване на неизправности при синхронизиране на [пароли с AZURE ad Connect Sync – не се синхронизират пароли](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c9e06-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="c9e06-110">**Синхронизирането на хеширане с парола не работи за някои от моите потребители**</span><span class="sxs-lookup"><span data-stu-id="c9e06-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="c9e06-111">Ако сте забелязали, че Хеширането на парола не се синхронизира за потребител, използвайте задачата за **отстраняване на неизправности** в Azure ad Connect, за да изследвате и отстраните проблема.</span><span class="sxs-lookup"><span data-stu-id="c9e06-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="c9e06-112">Изпълнете следните задачи:</span><span class="sxs-lookup"><span data-stu-id="c9e06-112">Perform the following tasks:</span></span>

    <span data-ttu-id="c9e06-113">на.</span><span class="sxs-lookup"><span data-stu-id="c9e06-113">a.</span></span> [<span data-ttu-id="c9e06-114">Изпълнение на задачата за отстраняване на неизправности в съветника</span><span class="sxs-lookup"><span data-stu-id="c9e06-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="c9e06-115">b.</span><span class="sxs-lookup"><span data-stu-id="c9e06-115">b.</span></span> [<span data-ttu-id="c9e06-116">Използвайте кратката команда за отстраняване на неизправности, за да изследвате проблема със синхронизирането на Хеширането на парола за конкретна употреба</span><span class="sxs-lookup"><span data-stu-id="c9e06-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="c9e06-117">Локалният потребителски обект Active Directory е разрешен, за **да може потребителят да смени паролата при следващото влизане** .</span><span class="sxs-lookup"><span data-stu-id="c9e06-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="c9e06-118">Когато тази опция е разрешена, на потребителя се присвоява временна парола и ще получите подкана да промените паролата при следващото влизане.</span><span class="sxs-lookup"><span data-stu-id="c9e06-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="c9e06-119">Свързването с Azure AD не синхронизира временните пароли в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9e06-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="c9e06-120">За да отстраните проблема по-горе, изпълнете една от следните задачи:</span><span class="sxs-lookup"><span data-stu-id="c9e06-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="c9e06-121">Помолете потребителя да влезе в локалното приложение (например настолната версия на Windows) и променете паролата.</span><span class="sxs-lookup"><span data-stu-id="c9e06-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="c9e06-122">Новата парола ще се синхронизира с Azure AD.</span><span class="sxs-lookup"><span data-stu-id="c9e06-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="c9e06-123">Помолете администратор да актуализира паролата на потребителя, без да позволява опцията **потребителят трябва да смени паролата си при следващото му влизане и да** сподели новата парола с потребителя.</span><span class="sxs-lookup"><span data-stu-id="c9e06-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="c9e06-124">Локалният потребителски обект Active Directory **не е конфигуриран правилно** за синхронизация на обекти или синхронизиране на парола.</span><span class="sxs-lookup"><span data-stu-id="c9e06-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="c9e06-125">За да отстраните този проблем, следвайте стъпките, описани в [отстраняването на неизправности при хеширане при синхронизиране с AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="c9e06-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







