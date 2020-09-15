---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697618"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="c0755-102">Active Directory не се синхронизира</span><span class="sxs-lookup"><span data-stu-id="c0755-102">Active Directory not syncing</span></span>

<span data-ttu-id="c0755-103">Ако получавате грешки при синхронизиране, като например "няма Последни синхронизации" или Забележка състоянието на синхронизиране на справочен указател в портала за администратори на Office казва "Последно синхронизиране повече от 3 дни назад", може да се окаже, че AADConnect има грешни настройки или недостатъчни разрешения за извършване на синхронизиране.</span><span class="sxs-lookup"><span data-stu-id="c0755-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="c0755-104">Преинсталирането на AADConnect с помощта на експресните настройки може бързо да отстрани проблема:</span><span class="sxs-lookup"><span data-stu-id="c0755-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="c0755-105">[Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="c0755-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="c0755-106">[Следвайте инструкциите за експресната инсталация](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="c0755-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="c0755-107">За повече информация за акаунтите за AADConnect Services вижте [AZURE ad Connect: акаунти и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="c0755-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
