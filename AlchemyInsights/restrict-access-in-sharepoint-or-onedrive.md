---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551440"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="74c5f-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="74c5f-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="74c5f-103">В SharePoint и OneDrive можете да ограничите достъпа до елементи като файлове, папки и списъци чрез предоставяне на достъп само за групи или лица, които искате да имате достъп.</span><span class="sxs-lookup"><span data-stu-id="74c5f-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="74c5f-104">По подразбиране разрешенията в SharePoint са наследени от по-високо в йерархията.</span><span class="sxs-lookup"><span data-stu-id="74c5f-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="74c5f-105">Така че файл наследява своите разрешения от папката, която наследява разрешенията си от библиотеката, която наследява разрешенията си от сайта.</span><span class="sxs-lookup"><span data-stu-id="74c5f-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="74c5f-106">Можете да споделяте на по-високо ниво (например чрез споделяне на цял сайт) и след това да го направите, ако не искате да споделяте всички елементи на сайта.</span><span class="sxs-lookup"><span data-stu-id="74c5f-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="74c5f-107">Въпреки това, ние не препоръчваме това, защото тя прави запазването на разрешенията по-сложни и объркващи в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="74c5f-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="74c5f-108">Ето какво можете да направите вместо това:</span><span class="sxs-lookup"><span data-stu-id="74c5f-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="74c5f-109">Ако например искате да споделите цялото съдържание на папка, с изключение на един файл в нея, преместете този файл на ново местоположение, което не е споделено.</span><span class="sxs-lookup"><span data-stu-id="74c5f-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="74c5f-110">Ако имате две подпапки в папка и искате да споделите една подпапка с групи A и B и да разрешите само група A достъп до втората подпапка, Споделете родителската папка с група а и добавете група б към първата подпапка.</span><span class="sxs-lookup"><span data-stu-id="74c5f-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="74c5f-111">Спиране на споделянето на файл или папка</span><span class="sxs-lookup"><span data-stu-id="74c5f-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

