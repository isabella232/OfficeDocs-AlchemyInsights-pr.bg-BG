---
title: Възстановяване на изтрит файл или папка
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1d9937c632212d12883a02860354b6112efd49a6
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36749897"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="32114-102">Възстановяване на изтрит файл или папка</span><span class="sxs-lookup"><span data-stu-id="32114-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="32114-103">SharePoint online запазва резервни копия на цялото съдържание за 14 допълнителни дни извън действителното изтриване.</span><span class="sxs-lookup"><span data-stu-id="32114-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="32114-104">Ако съдържанието не може да бъде възстановено чрез "Кошче" или "възстановяване на файлове", администраторът може да се свърже с поддръжката на Microsoft, за да изиска възстановяване по всяко време в рамките на 14-дневния прозорец.</span><span class="sxs-lookup"><span data-stu-id="32114-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="32114-105">Възстановявания от архиви могат да бъдат завършени само за колекции от сайтове или под-сайтове, а не за конкретни файлове, списъци или библиотеки.</span><span class="sxs-lookup"><span data-stu-id="32114-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="32114-106">Когато изтривате елемент или сайт от SharePoint, той не се отстранява незабавно.</span><span class="sxs-lookup"><span data-stu-id="32114-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="32114-107">Изтритите елементи влизат в кошчето за определен период от време.</span><span class="sxs-lookup"><span data-stu-id="32114-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="32114-108">През това време можете да възстановите елементите, които сте изтрили, в първоначалното им местоположение.</span><span class="sxs-lookup"><span data-stu-id="32114-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="32114-109">За повече информация, моля, посетете връзките по-долу.</span><span class="sxs-lookup"><span data-stu-id="32114-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="32114-110">[Възстановяване на елементи в кошчето на сайт на SharePoint](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="32114-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="32114-111">Възстановяване на изтрити файлове или папки в OneDrive</span><span class="sxs-lookup"><span data-stu-id="32114-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="32114-112">Възстановяване на изтрита колекция от сайтове (включително група, комуникация и други сайтове)</span><span class="sxs-lookup"><span data-stu-id="32114-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="32114-113">Възстановяване на изтрит сайт за OneDrive</span><span class="sxs-lookup"><span data-stu-id="32114-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="32114-114">За групово Кошче действия администраторите може да помислите за използване на [SharePoint online ПНП](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="32114-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="32114-115">**Функция за възстановяване на файлове**</span><span class="sxs-lookup"><span data-stu-id="32114-115">**Files Restore feature**</span></span>

<span data-ttu-id="32114-116">Ако много от вашите OneDrive или SharePoint файлове бъдат изтрити, заместени, повредени или заразени от злонамерен софтуер, можете да възстановите целия OneDrive или SharePoint библиотеката до предишно време с помощта на функцията за възстановяване на файлове.</span><span class="sxs-lookup"><span data-stu-id="32114-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="32114-117">Възстановяване на библиотека в OneDrive</span><span class="sxs-lookup"><span data-stu-id="32114-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="32114-118">Възстановяване на библиотека с документи</span><span class="sxs-lookup"><span data-stu-id="32114-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

