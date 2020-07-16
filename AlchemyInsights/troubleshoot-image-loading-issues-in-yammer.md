---
title: Отстраняване на неизправности при зареждане на изображения в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148170"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="4d236-102">Отстраняване на неизправности при зареждане на изображения в Yammer</span><span class="sxs-lookup"><span data-stu-id="4d236-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="4d236-103">Когато възникнат проблеми с снимки и визуализация на файлове в Yammer, отстраняване на неизправности чрез проверка дали проблемът възниква за всички потребители, дали той възниква на мобилни устройства и дали е възпроизводимо при качване на прикачения файл.</span><span class="sxs-lookup"><span data-stu-id="4d236-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="4d236-104">**Проблеми със снимката на профила**</span><span class="sxs-lookup"><span data-stu-id="4d236-104">**Profile photo issues**</span></span>  

<span data-ttu-id="4d236-105">Ако крайните потребители влизат в Yammer чрез Microsoft 365, те трябва да променят профила си, включително профилната снимка.</span><span class="sxs-lookup"><span data-stu-id="4d236-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="4d236-106">Ако потребителите нямат право да правят актуализации на профила, администраторът може да направи актуализацията за потребителя.</span><span class="sxs-lookup"><span data-stu-id="4d236-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="4d236-107">За повече информация вижте [Преглед и актуализиране на профила в Office delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="4d236-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="4d236-108">За информация относно редактирането на профил, включително снимки на потребителски профили, вижте [Промяна на моя профил и настройки на Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="4d236-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="4d236-109">Актуализираните снимки на потребителския профил се синхронизират по различен начин от атрибутите на профила.</span><span class="sxs-lookup"><span data-stu-id="4d236-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="4d236-110">Потребителите трябва да се регистрират, за да инициират синхронизиране на снимката на профила си.</span><span class="sxs-lookup"><span data-stu-id="4d236-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="4d236-111">За информация вижте [потребителски профил картини, актуализирани от Office 365 на Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="4d236-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="4d236-112">За информация относно жизнения цикъл на потребителя за Yammer вижте [Управление на yammer потребители през техния жизнен цикъл от Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="4d236-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="4d236-113">За подробности относно начина на работа на синхронизирането на профилни карти в Microsoft 365 вижте [информация за синхронизиране на картини на профили в Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="4d236-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="4d236-114">**Проблеми с прегледа на документи и миниатюри на изображения**</span><span class="sxs-lookup"><span data-stu-id="4d236-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="4d236-115">Когато файлове или изображения са публикувани в Yammer, визуализация може да не се появи, защото:</span><span class="sxs-lookup"><span data-stu-id="4d236-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="4d236-116">Файлът е повреден и не може да бъде обработен.</span><span class="sxs-lookup"><span data-stu-id="4d236-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="4d236-117">Файлът не е качен наскоро в SharePoint Online или Yammer има невалидни метаданни по други причини.</span><span class="sxs-lookup"><span data-stu-id="4d236-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="4d236-118">Url адресите, необходими за зареждане на изображенията за визуализация, са блокирани.</span><span class="sxs-lookup"><span data-stu-id="4d236-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="4d236-119">Визуализацията на файла е премахната от потребителя преди публикуването.</span><span class="sxs-lookup"><span data-stu-id="4d236-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="4d236-120">Проблем с услугата попречи на визуализацията да се генерира.</span><span class="sxs-lookup"><span data-stu-id="4d236-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="4d236-121">**Забележка:** Визуализациите за връзки и качени файлове може да се държат по различен начин.</span><span class="sxs-lookup"><span data-stu-id="4d236-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="4d236-122">Връзки към файлове в интернет или връзки, които изискват допълнително удостоверяване може да не се показват правилно.</span><span class="sxs-lookup"><span data-stu-id="4d236-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="4d236-123">За повече информация вижте [Прикачване на файл или изображение към съобщение на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="4d236-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 