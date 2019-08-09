---
title: Отстраняване на неизправности при "Отваряне с Explorer" в SharePoint Online
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: afee367e250357b20b77f0ea5dfe66d68967eb2a
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270697"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b920c-102">Отстраняване на неизправности при "Отваряне с Explorer" в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b920c-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="b920c-103">Командата "Отваряне с Explorer" отваря локален екземпляр на Windows Explorer, който показва структурата на папките на сървъра, хостващ сайта на SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b920c-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="b920c-104">По този начин, препоръчваме [синхронизиране на файлове на SharePoint с новия клиент за синхронизиране на OneDrive](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, който предоставя [Файлове при поискване](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), защото предоставя локален достъп до вашите файлове и предлага най-добро представяне.</span><span class="sxs-lookup"><span data-stu-id="b920c-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="b920c-105">Ако сте избрали да използвате изглед на Explorer, вместо да използвате новия клиент за синхронизиране на OneDrive, погрижете се да следвате стъпките и най-добрите практики в следните статии:</span><span class="sxs-lookup"><span data-stu-id="b920c-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b920c-106">Как да използвате командата "Отваряне с Explorer" за отстраняване на неизправности в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="b920c-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="b920c-107">Копиране или преместване на файлове в библиотеката чрез опцията "Отваряне с Explorer"</span><span class="sxs-lookup"><span data-stu-id="b920c-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="b920c-108">Бутонът **Отваряне с Explorer** не се появява в новия изглед на библиотеката.</span><span class="sxs-lookup"><span data-stu-id="b920c-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b920c-109">Изберете падащия списък **Изглед** в горния десен ъгъл (името на падащия списък се променя в зависимост от вашия текущ изглед), след което изберете **Изглед** във File Explorer.</span><span class="sxs-lookup"><span data-stu-id="b920c-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="b920c-110">SharePoint Отвори с Explorer използва ActiveX контроли, така че се поддържа само в Internet Explorer 10 или 11.</span><span class="sxs-lookup"><span data-stu-id="b920c-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b920c-111">Отвори с Explorer не работи в Windows с Microsoft Edge, Google Chrome, Mozilla Firefox или платформата Mac.</span><span class="sxs-lookup"><span data-stu-id="b920c-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b920c-112">Поради тази причина опцията за изглед на Explorer може да е в сив цвят.</span><span class="sxs-lookup"><span data-stu-id="b920c-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="b920c-113">[Защо бутоните на лентата на SharePoint са недостъпни или в сив цвят.](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="b920c-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

