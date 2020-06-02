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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511965"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a0cea-102">Не може да се изтрият елементи</span><span class="sxs-lookup"><span data-stu-id="a0cea-102">Unable to delete items</span></span>

<span data-ttu-id="a0cea-103">Правилата за задържане могат да причинят това, трябва да забраните или изключите съответното задържане, което причинява този проблем.</span><span class="sxs-lookup"><span data-stu-id="a0cea-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a0cea-104">След като правило за задържане или задържане е премахната, промяната може да отнеме до 24 часа.</span><span class="sxs-lookup"><span data-stu-id="a0cea-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="a0cea-105">Уверете се, че няма настройка на [правилата за задържане](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) на елемента.</span><span class="sxs-lookup"><span data-stu-id="a0cea-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="a0cea-106">Сайтът може да е надвишил ограничението за съхранение, да увеличи [квотата](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) на сайта и да изтрие елемента.</span><span class="sxs-lookup"><span data-stu-id="a0cea-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="a0cea-107">Уверете се, че елементът не е [извлечен от](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) друг потребител.</span><span class="sxs-lookup"><span data-stu-id="a0cea-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="a0cea-108">И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), който съдържа библиотека на PowerShell команди, които ви позволяват да извършвате сложни действия за управление като принудително изтриване на упорити елементи.</span><span class="sxs-lookup"><span data-stu-id="a0cea-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a0cea-109">Премахване на PNP файл</span><span class="sxs-lookup"><span data-stu-id="a0cea-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a0cea-110">Премахване на PNP папка</span><span class="sxs-lookup"><span data-stu-id="a0cea-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a0cea-111">Премахване на елемент от списъка с PNP</span><span class="sxs-lookup"><span data-stu-id="a0cea-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a0cea-112">Премахване на списъка с PNP</span><span class="sxs-lookup"><span data-stu-id="a0cea-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a0cea-113">Премахване на PNP поле (колона)</span><span class="sxs-lookup"><span data-stu-id="a0cea-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)