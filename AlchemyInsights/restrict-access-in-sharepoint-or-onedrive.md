---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720671"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="74854-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="74854-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="74854-103">В SharePoint и OneDrive можете да ограничите достъпа до елементи, като например файлове, папки и списъци, като предоставите достъп само до групи или лица, на които искате да имате достъп.</span><span class="sxs-lookup"><span data-stu-id="74854-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="74854-104">По подразбиране разрешенията в SharePoint се наследяват от по-високо в йерархията.</span><span class="sxs-lookup"><span data-stu-id="74854-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="74854-105">Така че един файл наследява разрешенията си от папката, която наследява разрешенията му от библиотеката, която наследява разрешенията му от сайта.</span><span class="sxs-lookup"><span data-stu-id="74854-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="74854-106">Можете да споделяте на по-високо ниво (например чрез споделяне на цял сайт), а след това да прекъснете наследяването, ако не искате да споделяте всички елементи в сайта.</span><span class="sxs-lookup"><span data-stu-id="74854-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="74854-107">Все пак не препоръчваме това, защото това улеснява поддържането на разрешенията по-сложни и объркващи в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="74854-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="74854-108">Ето какво можете да направите вместо това:</span><span class="sxs-lookup"><span data-stu-id="74854-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="74854-109">Ако например искате да споделите цялото съдържание на папка, с изключение на един файл в нея, пренесете този файл в ново местоположение, което не е споделено.</span><span class="sxs-lookup"><span data-stu-id="74854-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="74854-110">Ако имате две подпапки в папка и искате да споделите една подпапка с групи а и б и да разрешите само групиране на достъп до втората подпапка, Споделете родителската папка с група A и добавете група B към първата подпапка.</span><span class="sxs-lookup"><span data-stu-id="74854-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="74854-111">Спиране на споделянето на файл или папка </span><span class="sxs-lookup"><span data-stu-id="74854-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

