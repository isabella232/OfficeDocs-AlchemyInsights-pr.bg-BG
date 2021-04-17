---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822840"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="09e8d-102">Active Directory не се синхронизира</span><span class="sxs-lookup"><span data-stu-id="09e8d-102">Active Directory not syncing</span></span>

<span data-ttu-id="09e8d-103">Ако получавате грешки при синхронизиране, като например "няма скорошно синхронизиране", или забележите състоянието на синхронизиране на справочен указател в портала за администриране на Office, "Последно синхронизирано преди повече от 3 дни", може да се окаже, че AADConnect има неправилни настройки или недостатъчни разрешения за извършване на синхронизиране.</span><span class="sxs-lookup"><span data-stu-id="09e8d-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="09e8d-104">Преинсталирането на AADConnect с помощта на експресни настройки може да реши проблема бързо:</span><span class="sxs-lookup"><span data-stu-id="09e8d-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="09e8d-105">[Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="09e8d-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="09e8d-106">[Следвайте инструкциите за експресна инсталация](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="09e8d-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="09e8d-107">За повече информация относно акаунтите за услуги на AADConnect вижте [Azure AD Connect: Акаунти и разрешения.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="09e8d-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
