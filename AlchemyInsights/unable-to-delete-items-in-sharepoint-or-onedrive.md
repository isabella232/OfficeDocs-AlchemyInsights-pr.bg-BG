---
title: Не може да се изтрият елементи в SharePoint или OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049506"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="01d19-102">Не могат да се изтрият елементи</span><span class="sxs-lookup"><span data-stu-id="01d19-102">Unable to delete items</span></span>

<span data-ttu-id="01d19-103">Имате проблеми с изтриването на елементи на SharePoint?</span><span class="sxs-lookup"><span data-stu-id="01d19-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="01d19-104">Винаги се уверете, че имате [съответните разрешения](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) за изтриване на елемента или имате опит да премахнете този елемент от [администратора на колекцията от сайтове](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) .</span><span class="sxs-lookup"><span data-stu-id="01d19-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="01d19-105">Уверете се, че няма настройка на [правилата за задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.</span><span class="sxs-lookup"><span data-stu-id="01d19-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="01d19-106">Уверете се, че елементът не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) за друг потребител.</span><span class="sxs-lookup"><span data-stu-id="01d19-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="01d19-107">И накрая, администраторите могат да използват [модели и практики на SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (ПНП), който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни управленски действия като сила изтриване на упорити елементи.</span><span class="sxs-lookup"><span data-stu-id="01d19-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="01d19-108">Премахване на ПНП файл</span><span class="sxs-lookup"><span data-stu-id="01d19-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="01d19-109">Премахване на ПНП папка</span><span class="sxs-lookup"><span data-stu-id="01d19-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="01d19-110">Премахни ПНП елемент от списък</span><span class="sxs-lookup"><span data-stu-id="01d19-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="01d19-111">Премахване на ПНП списък</span><span class="sxs-lookup"><span data-stu-id="01d19-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="01d19-112">Премахване на ПНП поле (колона)</span><span class="sxs-lookup"><span data-stu-id="01d19-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)