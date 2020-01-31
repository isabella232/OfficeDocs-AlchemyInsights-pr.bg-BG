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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571222"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="1c201-102">Не може да се изтрият елементи</span><span class="sxs-lookup"><span data-stu-id="1c201-102">Unable to delete items</span></span>

<span data-ttu-id="1c201-103">Правила за задържане може да доведе до това, трябва да забраните или изключите съответното задържане, което причинява този проблем.</span><span class="sxs-lookup"><span data-stu-id="1c201-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="1c201-104">След премахването на правило или задържане, може да отнеме до 24 часа, за да влязат в сила промяната.</span><span class="sxs-lookup"><span data-stu-id="1c201-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="1c201-105">Уверете се, че няма настройка на правила за [задържане](https://docs.microsoft.com/office365/securitycompliance/retention-policies) на елемента.</span><span class="sxs-lookup"><span data-stu-id="1c201-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="1c201-106">Сайтът може да е надвишил лимита за съхранение, да увеличи [квотата](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) на сайта и да изтрие елемента.</span><span class="sxs-lookup"><span data-stu-id="1c201-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="1c201-107">Уверете се, че елементът не е [извлечен](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) на друг потребител.</span><span class="sxs-lookup"><span data-stu-id="1c201-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="1c201-108">И накрая администраторите могат да използват [SharePoint модели и практики](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), която съдържа библиотека от PowerShell команди, които ви позволяват да извършвате сложни действия за управление като сила изтриване на упорити елементи.</span><span class="sxs-lookup"><span data-stu-id="1c201-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="1c201-109">Премахване на PNP файл</span><span class="sxs-lookup"><span data-stu-id="1c201-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="1c201-110">Премахни папката PNP</span><span class="sxs-lookup"><span data-stu-id="1c201-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="1c201-111">Премахване на елемент от списък с PNP</span><span class="sxs-lookup"><span data-stu-id="1c201-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="1c201-112">Премахване на списък с PNP</span><span class="sxs-lookup"><span data-stu-id="1c201-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="1c201-113">Премахване на PNP поле (колона)</span><span class="sxs-lookup"><span data-stu-id="1c201-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)