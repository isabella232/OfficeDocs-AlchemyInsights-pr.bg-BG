---
title: Закъснения при получаване на известия на SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727232"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="0662f-102">Закъснения при получаване на известия на SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="0662f-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="0662f-103">Първо проверете папката Нежелана поща в имейла.</span><span class="sxs-lookup"><span data-stu-id="0662f-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="0662f-104">Ако **всички предупреждения от множество файлове или библиотеки са закъснели**, отидете на [таблото за изправност на услугите](https://portal.office.com/adminportal/home?ref=/servicehealth) , за да проверите за всички съвети/събития, които може да възникнат при SharePoint или Exchange.</span><span class="sxs-lookup"><span data-stu-id="0662f-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="0662f-105">Възможно е проблемът да е в възможностите за уведомяване на SharePoint или закъсненията в имейли чрез Exchange.</span><span class="sxs-lookup"><span data-stu-id="0662f-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="0662f-106">Също така имайте предвид, че ако не е получено друго имейл съобщение, проблемът е вероятен при закъснения на Exchange.</span><span class="sxs-lookup"><span data-stu-id="0662f-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="0662f-107">Ако **не е дадено отделно известие от конкретен файл или библиотека**, опитайте да го изтриете и пресъздадете.</span><span class="sxs-lookup"><span data-stu-id="0662f-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="0662f-108">Вижте [управление, преглед или изтриване на известия на SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) , за да създадете отново известието.</span><span class="sxs-lookup"><span data-stu-id="0662f-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="0662f-109">Известията не могат да бъдат изпратени до група за разпространение.</span><span class="sxs-lookup"><span data-stu-id="0662f-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="0662f-110">Поддържат се само групи за защита и O365.</span><span class="sxs-lookup"><span data-stu-id="0662f-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="0662f-111">Не можете да персонализирате шаблоните за имейл известия.</span><span class="sxs-lookup"><span data-stu-id="0662f-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="0662f-112">Трябва да използвате Microsoft Flow или SharePoint Designer Workflow, за да ги постигнете.</span><span class="sxs-lookup"><span data-stu-id="0662f-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
