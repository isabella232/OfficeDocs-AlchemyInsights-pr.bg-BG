---
title: Не може да изтрие елементи в SharePoint или OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 82a19c8ea218834b71901e95747da0c99243893e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757914"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="8dcd3-102">Не може да изтрие елементи</span><span class="sxs-lookup"><span data-stu-id="8dcd3-102">Unable to delete items</span></span>

<span data-ttu-id="8dcd3-103">Като проблеми, изтриване на елементи?</span><span class="sxs-lookup"><span data-stu-id="8dcd3-103">Having issues deleting items?</span></span>

- <span data-ttu-id="8dcd3-104">Винаги се уверете, че имате [необходимите разрешения](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) да изтриете елемента или [администраторът на колекцията сайтове](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) опит премахнете елемента.</span><span class="sxs-lookup"><span data-stu-id="8dcd3-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="8dcd3-105">Гарантира, че няма настройка на [правила за задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.</span><span class="sxs-lookup"><span data-stu-id="8dcd3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="8dcd3-106">Гарантира елемент не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) при друг потребител.</span><span class="sxs-lookup"><span data-stu-id="8dcd3-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="8dcd3-107">И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни управление действия като сила изтриване упорит елементи.</span><span class="sxs-lookup"><span data-stu-id="8dcd3-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="8dcd3-108">Премахнете PNP файл</span><span class="sxs-lookup"><span data-stu-id="8dcd3-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="8dcd3-109">Премахване на PNP папка</span><span class="sxs-lookup"><span data-stu-id="8dcd3-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="8dcd3-110">Премахване на елемент от PNP списък</span><span class="sxs-lookup"><span data-stu-id="8dcd3-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="8dcd3-111">Премахване на PNP списък</span><span class="sxs-lookup"><span data-stu-id="8dcd3-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="8dcd3-112">Премахнете PNP поле (колона)</span><span class="sxs-lookup"><span data-stu-id="8dcd3-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)