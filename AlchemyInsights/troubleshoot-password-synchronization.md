---
title: Отстраняване на неизправности при синхронизиране на пароли
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732499"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="666bf-102">Отстраняване на неизправности при синхронизиране на пароли</span><span class="sxs-lookup"><span data-stu-id="666bf-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="666bf-103">За отстраняване на проблеми, при които няма пароли се синхронизират с Azure AD свързване на версия 1.1.614.0 или по-късно:</span><span class="sxs-lookup"><span data-stu-id="666bf-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="666bf-104">Отворете нов Windows PowerShell сесия на azure AD свързване сървър с опцията **Изпълни като администратор** .</span><span class="sxs-lookup"><span data-stu-id="666bf-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="666bf-105">Изпълнение **на набор изпълнениеPolicy RemoteSigned** или **Задаване изпълнениеполитика неограничен .**</span><span class="sxs-lookup"><span data-stu-id="666bf-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="666bf-106">Стартирайте съветника за свързване на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="666bf-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="666bf-107">Отидете на страницата **Допълнителни задачи,** изберете **Отстраняване на неизправности**и щракнете върху **Напред**.</span><span class="sxs-lookup"><span data-stu-id="666bf-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="666bf-108">На страницата отстраняване на неизправности щракнете върху **Стартиране, за да стартирате менюто за отстраняване на неизправности** в PowerShell.</span><span class="sxs-lookup"><span data-stu-id="666bf-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="666bf-109">В главното меню изберете **Отстраняване на неизправности при синхронизиране на пароли**.</span><span class="sxs-lookup"><span data-stu-id="666bf-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="666bf-110">В подменюто изберете **Синхронизиране на пароли изобщо не работи**.</span><span class="sxs-lookup"><span data-stu-id="666bf-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="666bf-111">**Разберете резултатите от задачата за отстраняване на неизправности**</span><span class="sxs-lookup"><span data-stu-id="666bf-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="666bf-112">Задачата за отстраняване на неизправности извършва следните проверки:</span><span class="sxs-lookup"><span data-stu-id="666bf-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="666bf-113">Проверява, че функцията за синхронизиране на пароли е разрешена за azure AD клиент.</span><span class="sxs-lookup"><span data-stu-id="666bf-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="666bf-114">Проверява дали Azure AD свързване сървър не е в режим на спиране.</span><span class="sxs-lookup"><span data-stu-id="666bf-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="666bf-115">За всеки съществуващ Active Directory конектор (който отговаря на съществуващ Active Directory гора):</span><span class="sxs-lookup"><span data-stu-id="666bf-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="666bf-116">Проверява дали функцията за синхронизиране на пароли е разрешена.</span><span class="sxs-lookup"><span data-stu-id="666bf-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="666bf-117">Търси за синхронизиране на пароли пулсации събития в регистрационните файлове на приложението на Windows.</span><span class="sxs-lookup"><span data-stu-id="666bf-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="666bf-118">За всеки домейн на Active Directory под локалната конектор за Active Directory:</span><span class="sxs-lookup"><span data-stu-id="666bf-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="666bf-119">Проверява, че домейнът е достъпен от Azure AD свързване сървър.</span><span class="sxs-lookup"><span data-stu-id="666bf-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="666bf-120">Проверява, че акаунтите на домейнови услуги на Active Directory (AD DS), използвани от локалния Конектор за Active Directory има правилно потребителско име, парола и разрешения за синхронизиране на пароли.</span><span class="sxs-lookup"><span data-stu-id="666bf-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="666bf-121">За повече помощ за отстраняване на синхронизиране на парола вижте [Отстраняване на неизправности синхронизиране на пароли с Azure AD свързване синхронизация](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="666bf-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  