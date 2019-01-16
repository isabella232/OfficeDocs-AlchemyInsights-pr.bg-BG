---
title: Ограничаване на достъпа в SharePoint или OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276318"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="4f3b2-102">Ограничаване на достъпа в SharePoint или OneDrive</span><span class="sxs-lookup"><span data-stu-id="4f3b2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="4f3b2-p101">В SharePoint и OneDrive да ограничи достъпа до елементи като файлове, папки и списъци чрез предоставяне на достъп само до групи или лица, които искате да имат достъп. По подразбиране разрешения в SharePoint са наследени от по-нагоре в йерархията. Така файл наследява разрешенията от папката, която наследява разрешенията от библиотеката, която наследява разрешенията от сайта.</span><span class="sxs-lookup"><span data-stu-id="4f3b2-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="4f3b2-p102">Можете да споделяте по-високо ниво (като например чрез споделяне на целия сайт) и след това почивка наследството, ако не искате да споделите всички елементи на сайта. Обаче ние не препоръчваме това, защото той прави поддържането на разрешения по-сложно и объркващо в бъдеще. Ето какво можете да направите вместо това:</span><span class="sxs-lookup"><span data-stu-id="4f3b2-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="4f3b2-109">Ако, например, искате да споделите цялото съдържание на една папка с изключение на един файл в нея, преместете файла на ново място, която не е споделена.</span><span class="sxs-lookup"><span data-stu-id="4f3b2-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="4f3b2-110">Ако имате две подпапки в папка, и искате да споделите един подпапка с групи A и Б и позволяват само група А достъп до втория подпапка, споделяне на родителската папка с група А и добавяне на група Б към първата подпапка.</span><span class="sxs-lookup"><span data-stu-id="4f3b2-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="4f3b2-111">Спри споделянето на файл или папка</span><span class="sxs-lookup"><span data-stu-id="4f3b2-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

