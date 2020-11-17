---
title: Отстраняване на неизправности при "Отваряне с Explorer" в SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086037"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="9515a-102">Отстраняване на неизправности при "Отваряне с Explorer" в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9515a-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="9515a-103">Следвайте стъпките и най-добрите практики в следните статии:</span><span class="sxs-lookup"><span data-stu-id="9515a-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="9515a-104">Как да използвате командата "Отваряне с Explorer" за отстраняване на неизправности в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="9515a-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="9515a-105">Копиране или преместване на файлове в библиотеката чрез опцията "Отваряне с Explorer"</span><span class="sxs-lookup"><span data-stu-id="9515a-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="9515a-106">Препоръчваме [синхронизирането на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) , който предоставя [файлове при поискване](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) , тъй като синхронизирането предоставя локален достъп до вашите файлове и предлага най-добра производителност.</span><span class="sxs-lookup"><span data-stu-id="9515a-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="9515a-107">**Отваряне с Explorer** се поддържа само в Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="9515a-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="9515a-108">За повече информация вижте [прекратяване на поддръжката за IE11 с приложения на Microsoft 365](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span><span class="sxs-lookup"><span data-stu-id="9515a-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="9515a-109">Опцията " **Отваряне с Explorer** " не работи в Windows с Microsoft Edge, Google Chrome, Mozilla Firefox или платформата за Mac.</span><span class="sxs-lookup"><span data-stu-id="9515a-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="9515a-110">Поради тази причина опцията за **изглед на Explorer** може да е сива.</span><span class="sxs-lookup"><span data-stu-id="9515a-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="9515a-111">Бутонът **Отваряне с Explorer** не се появява в новия изглед на библиотеката.</span><span class="sxs-lookup"><span data-stu-id="9515a-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="9515a-112">Изберете падащия списък **Изглед** в горния десен ъгъл (името на падащия списък се променя в зависимост от вашия текущ изглед), след което изберете **Изглед** във File Explorer.</span><span class="sxs-lookup"><span data-stu-id="9515a-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

