---
title: Отстраняване на проблеми с зареждането на изображение в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690232"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="d6617-102">Отстраняване на проблеми с зареждането на изображение в Yammer</span><span class="sxs-lookup"><span data-stu-id="d6617-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="d6617-103">Когато проблемите възникват със снимки и визуализации на файлове в Yammer, отстраняване на неизправности чрез проверка дали проблемът възниква за всички потребители, дали възниква на мобилни устройства, и дали е възпроизводим при качване на прикачения файл.</span><span class="sxs-lookup"><span data-stu-id="d6617-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="d6617-104">**Проблеми със снимките в профила**</span><span class="sxs-lookup"><span data-stu-id="d6617-104">**Profile photo issues**</span></span>  

<span data-ttu-id="d6617-105">Ако крайните потребители влизат в Yammer чрез Microsoft 365, те трябва да променят профила си, включително снимката в профила си.</span><span class="sxs-lookup"><span data-stu-id="d6617-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="d6617-106">Ако потребителите не могат да правят актуализации на профила, администраторът може да направи актуализацията за потребителя.</span><span class="sxs-lookup"><span data-stu-id="d6617-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="d6617-107">За повече информация вижте [Преглед и актуализиране на вашия профил в Office delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="d6617-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="d6617-108">За информация за редактирането на профили, включително снимки на профила, вижте [Промяна на моя профил и настройки на Yammer](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="d6617-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="d6617-109">Актуализиран профил снимките са синхронизирани по различен начин от атрибутите на профила.</span><span class="sxs-lookup"><span data-stu-id="d6617-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="d6617-110">Потребителите трябва да влязат, за да започнат синхронизиране на своята снимка на профила.</span><span class="sxs-lookup"><span data-stu-id="d6617-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="d6617-111">За повече информация вижте [снимки на потребителски профил, актуализирани от Office 365 към Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="d6617-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="d6617-112">За информация за жизнения цикъл на потребителите за Yammer вижте [управление на потребители на Yammer през целия им жизнен цикъл от Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="d6617-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="d6617-113">За подробности относно синхронизирането на картини в профил в Microsoft 365 вижте [информация за синхронизирането на картини в профила в microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="d6617-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="d6617-114">**Изображение на лентата на Excel**</span><span class="sxs-lookup"><span data-stu-id="d6617-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="d6617-115">Когато файловете или изображенията са публикувани в Yammer, може да не се показват визуализации, тъй като:</span><span class="sxs-lookup"><span data-stu-id="d6617-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="d6617-116">Файлът е повреден и не може да бъде обработен.</span><span class="sxs-lookup"><span data-stu-id="d6617-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="d6617-117">Файлът не е бил наскоро качен в SharePoint Online или Yammer има невалидни метаданни по други причини.</span><span class="sxs-lookup"><span data-stu-id="d6617-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="d6617-118">URL адресите, необходими за зареждане на изображенията на предварителния преглед, се блокират.</span><span class="sxs-lookup"><span data-stu-id="d6617-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="d6617-119">Визуализацията на файла е премахната от потребителя преди осчетоводяването.</span><span class="sxs-lookup"><span data-stu-id="d6617-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="d6617-120">Проблем с услугата попречи на генерирането на визуализация.</span><span class="sxs-lookup"><span data-stu-id="d6617-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="d6617-121">**Забележка** Визуализациите за връзки и качването на файлове може да се държат различно.</span><span class="sxs-lookup"><span data-stu-id="d6617-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="d6617-122">Връзки към файлове в интернет или връзки, изискващи допълнително удостоверяване, може да не се показват правилно.</span><span class="sxs-lookup"><span data-stu-id="d6617-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="d6617-123">За повече информация вижте [Прикачване на файл или изображение към съобщение на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="d6617-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 