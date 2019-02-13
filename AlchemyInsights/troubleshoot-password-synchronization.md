---
title: Отстраняване на неизправности при синхронизиране на пароли
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924685"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="3d94f-102">Отстраняване на неизправности при синхронизиране на пароли</span><span class="sxs-lookup"><span data-stu-id="3d94f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="3d94f-103">За отстраняване на проблеми, където не пароли са синхронизирани с Azure АД свържете версия 1.1.614.0 или по-късно:</span><span class="sxs-lookup"><span data-stu-id="3d94f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="3d94f-104">Отворете нова сесия на Windows PowerShell на вашия сървър, Azure АД се свързват с опцията **Изпълни като администратор** .</span><span class="sxs-lookup"><span data-stu-id="3d94f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="3d94f-105">Тичам **комплект-ExecutionPolicy RemoteSigned** или **комплект-ExecutionPolicy неограничен**.</span><span class="sxs-lookup"><span data-stu-id="3d94f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="3d94f-106">Стартирайте съветника за Azure АД се свържете.</span><span class="sxs-lookup"><span data-stu-id="3d94f-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="3d94f-107">Навигирайте до \*\* допълнителни задачи \*\* страница, изберете \*\* отстраняване на \*\* и щракнете върху **напред**.</span><span class="sxs-lookup"><span data-stu-id="3d94f-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="3d94f-108">Отстраняване на неизправности в страницата щракнете върху **стартирането да започне отстраняване на** менюто в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3d94f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="3d94f-109">В главното меню изберете **Отстраняване на неизправности при синхронизиране на пароли**.</span><span class="sxs-lookup"><span data-stu-id="3d94f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="3d94f-110">В менюто под изберете **парола не работи изобщо**.</span><span class="sxs-lookup"><span data-stu-id="3d94f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="3d94f-111">**Разбиране на резултатите от отстраняване на задачата**</span><span class="sxs-lookup"><span data-stu-id="3d94f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="3d94f-112">Отстраняване на задачата извършва следните проверки:</span><span class="sxs-lookup"><span data-stu-id="3d94f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="3d94f-113">Утвърждава, че функцията за синхронизиране на паролата е разрешено за вашия лазурно АД наемател.</span><span class="sxs-lookup"><span data-stu-id="3d94f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="3d94f-114">Утвърждава че Azure АД свържете сървър не е в режим за спиране.</span><span class="sxs-lookup"><span data-stu-id="3d94f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="3d94f-115">За всеки съществуващ на локалната Active Directory съединител, (което отговаря на съществуващата структура на Active Directory):</span><span class="sxs-lookup"><span data-stu-id="3d94f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="3d94f-116">Проверява дали е разрешена функцията за синхронизиране на паролата.</span><span class="sxs-lookup"><span data-stu-id="3d94f-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="3d94f-117">Търси за парола synchronization сърцебиене събития в регистрационни файлове Windows приложение.</span><span class="sxs-lookup"><span data-stu-id="3d94f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="3d94f-118">За всеки Active Directory домейн под конектора на локалната Active Directory:</span><span class="sxs-lookup"><span data-stu-id="3d94f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="3d94f-119">Утвърждава, че домейна е достижима от Azure АД се свържете сървъра.</span><span class="sxs-lookup"><span data-stu-id="3d94f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="3d94f-120">Утвърждава че услуги за домейн на Active Directory (AD DS) акаунти, използвани от локалната Active Directory съединителя е правилното потребителско име, парола и разрешения, необходими за синхронизиране на пароли.</span><span class="sxs-lookup"><span data-stu-id="3d94f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="3d94f-121">За повече помощ, отстраняване на парола sync вижте [отстраняване парола синхронизация с Azure АД свържете синхронизация](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3d94f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

