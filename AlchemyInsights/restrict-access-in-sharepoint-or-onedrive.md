---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715873"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="0a7e1-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="0a7e1-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="0a7e1-103">В SharePoint и OneDrive можете да ограничите достъпа до елементи като файлове, папки и списъци чрез предоставяне на достъп само на групи или лица, които искате да имате достъп.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="0a7e1-104">По подразбиране разрешенията в SharePoint се наследяват от по-горе в йерархията.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="0a7e1-105">Така файлът наследява своите разрешения от папката, която наследява нейните разрешения от библиотеката, която наследява разрешенията му от сайта.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="0a7e1-106">Можете да споделяте на по-високо ниво (например чрез споделяне на цял сайт) и след това да прекъснете наследяването, ако не искате да споделяте всички елементи в сайта.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="0a7e1-107">Въпреки това, ние не препоръчваме това, защото прави поддържането на разрешенията по-сложно и объркващо в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="0a7e1-108">Ето какво бихте могли да направите вместо това:</span><span class="sxs-lookup"><span data-stu-id="0a7e1-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="0a7e1-109">Ако например искате да споделите цялото съдържание на папка, с изключение на един файл в нея, преместете файла на ново местоположение, което не е споделено.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="0a7e1-110">Ако имате две подпапки в папка и искате да споделите една подпапка с групи А и Б и позволи те да имат достъп само до втората подпапка, споделете родителската папка с група A и добавете група B към първата подпапка.</span><span class="sxs-lookup"><span data-stu-id="0a7e1-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="0a7e1-111">Спиране на споделянето на файл или папка</span><span class="sxs-lookup"><span data-stu-id="0a7e1-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

