---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265130"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="1a4e6-102">Active Directory не се синхронизира</span><span class="sxs-lookup"><span data-stu-id="1a4e6-102">Active Directory not syncing</span></span>

<span data-ttu-id="1a4e6-103">Ако получавате грешки при синхронизацията, като например "няма скорошно синхронизиране" или забележите състоянието на синхронизиране на директории в портала за администриране на Office казва" последно синхронизирани преди повече от 3 дни," това може да е, че AADConnect има неправилни настройки или недостатъчно разрешения за извършване на синхронизация.</span><span class="sxs-lookup"><span data-stu-id="1a4e6-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="1a4e6-104">Преинсталиране на AADConnect чрез бързи настройки може да реши проблема бързо:</span><span class="sxs-lookup"><span data-stu-id="1a4e6-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="1a4e6-105">[Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="1a4e6-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="1a4e6-106">[Следвайте инструкциите за експресно инсталиране](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="1a4e6-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="1a4e6-107">За повече информация относно AADConnect сервизни акаунти вижте [Azure AD свързване: акаунти и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="1a4e6-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
