---
title: Собственикът не може да създаде подпапка с помощта на Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/12/2020
ms.locfileid: "44748733"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="c6a31-102">Собственикът не може да създаде подпапка с помощта на Outlook</span><span class="sxs-lookup"><span data-stu-id="c6a31-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="c6a31-103">**Има текущ проблем със собствениците на публична папка, създаващи подпапки с помощта на Outlook. Проблемът скоро ще бъде решен.**</span><span class="sxs-lookup"><span data-stu-id="c6a31-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="c6a31-104">Междувременно използвайте един от следните методи:</span><span class="sxs-lookup"><span data-stu-id="c6a31-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="c6a31-105">Използвайте Outlook за MAC, за да създадете подпапка като проблем засяга само Outlook за настолни прозорци (всички версии)</span><span class="sxs-lookup"><span data-stu-id="c6a31-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="c6a31-106">Да администратор създаде подпапка с помощта на EXO Shell или EAC</span><span class="sxs-lookup"><span data-stu-id="c6a31-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="c6a31-107">Промяна на DefaultPublicFolderMailbox/EffectivePublicFolderMailbox на потребителя пощенска кутия на друга пощенска кутия за съдържание за папката, причиняваща проблем</span><span class="sxs-lookup"><span data-stu-id="c6a31-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="c6a31-108">*Потребителската настройка на потребителската папка по подразбиранеPublicNamebox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="c6a31-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="c6a31-109">Изчакайте един час, рестартирайте клиента на Outlook</span><span class="sxs-lookup"><span data-stu-id="c6a31-109">Wait for an hour, restart outlook client</span></span>