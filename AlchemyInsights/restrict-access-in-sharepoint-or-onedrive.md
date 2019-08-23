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
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551440"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="a4589-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="a4589-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="a4589-103">В SharePoint и OneDrive да ограничи достъпа до елементи като файлове, папки и списъци чрез предоставяне на достъп само до групи или лица, които искате да имат достъп.</span><span class="sxs-lookup"><span data-stu-id="a4589-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="a4589-104">По подразбиране разрешения в SharePoint са наследени от по-нагоре в йерархията.</span><span class="sxs-lookup"><span data-stu-id="a4589-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="a4589-105">Така файл наследява разрешенията от папката, която наследява разрешенията от библиотеката, която наследява разрешенията от сайта.</span><span class="sxs-lookup"><span data-stu-id="a4589-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="a4589-106">Можете да споделяте по-високо ниво (като например чрез споделяне на целия сайт) и след това почивка наследството, ако не искате да споделите всички елементи на сайта.</span><span class="sxs-lookup"><span data-stu-id="a4589-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="a4589-107">Обаче ние не препоръчваме това, защото той прави поддържането на разрешения по-сложно и объркващо в бъдеще.</span><span class="sxs-lookup"><span data-stu-id="a4589-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="a4589-108">Ето какво можете да направите вместо това:</span><span class="sxs-lookup"><span data-stu-id="a4589-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="a4589-109">Ако, например, искате да споделите цялото съдържание на една папка с изключение на един файл в нея, преместете файла на ново място, която не е споделена.</span><span class="sxs-lookup"><span data-stu-id="a4589-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="a4589-110">Ако имате две подпапки в папка, и искате да споделите един подпапка с групи A и Б и позволяват само група А достъп до втория подпапка, споделяне на родителската папка с група А и добавяне на група Б към първата подпапка.</span><span class="sxs-lookup"><span data-stu-id="a4589-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="a4589-111">Спри споделянето на файл или папка</span><span class="sxs-lookup"><span data-stu-id="a4589-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

