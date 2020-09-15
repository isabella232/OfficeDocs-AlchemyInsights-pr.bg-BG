---
title: Отстраняване на неизправности при синхронизиране на парола
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664915"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="43fe8-102">Отстраняване на неизправности при синхронизиране на парола</span><span class="sxs-lookup"><span data-stu-id="43fe8-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="43fe8-103">За отстраняване на проблеми при синхронизиране на парола започнете с помощта на тази задача за отстраняване на неизправности с "пад", за да определите защо паролите не се синхронизират.</span><span class="sxs-lookup"><span data-stu-id="43fe8-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="43fe8-104">За да започнете, отидете на [управление на директното синхронизиране](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="43fe8-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="43fe8-105">Отворете нова сесия на Windows PowerShell на вашия сървър на Azure AD Connect и изберете опцията **Изпълнявай като администратор** .</span><span class="sxs-lookup"><span data-stu-id="43fe8-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="43fe8-106">Run Set-ExecutionPolicy RemoteSigned или Set-ExecutionPolicy неограничени.</span><span class="sxs-lookup"><span data-stu-id="43fe8-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="43fe8-107">Стартирайте съветника за свързване на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="43fe8-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="43fe8-108">Отиване на страницата с допълнителни задачи > **отстраняване на неизправности**  >  **след**това.</span><span class="sxs-lookup"><span data-stu-id="43fe8-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="43fe8-109">Изберете **стартиране** , за да отворите менюто отстраняване на неизправности на PowerShell.</span><span class="sxs-lookup"><span data-stu-id="43fe8-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="43fe8-110">Изберете **отстраняване на неизправности при синхронизиране на парола**.</span><span class="sxs-lookup"><span data-stu-id="43fe8-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="43fe8-111">Обикновено проблемът е, че една парола не е синхронизирана за конкретен потребителски акаунт.</span><span class="sxs-lookup"><span data-stu-id="43fe8-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="43fe8-112">**Бележки** Синхронизирането на парола е неуспешно, ако последното успешно синхронизиране на парола е било преди известно време.</span><span class="sxs-lookup"><span data-stu-id="43fe8-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="43fe8-113">За повече помощ за отстраняване на неизправности при синхронизиране на парола вижте [отстраняване на неизправности при хеширане с криптиране чрез AZURE ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="43fe8-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>