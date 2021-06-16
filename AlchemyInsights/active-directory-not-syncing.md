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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930964"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="f6180-102">Active Directory не се синхронизира</span><span class="sxs-lookup"><span data-stu-id="f6180-102">Active Directory not syncing</span></span>

<span data-ttu-id="f6180-103">Ако получавате грешки при синхронизиране, като например "няма скорошно синхронизиране", или забележите състоянието на синхронизиране на справочен указател в портала за администриране на Office казва "Последно синхронизирано преди повече от 3 дни", може да се окаже, че AADConnect има неправилни настройки или недостатъчни разрешения за извършване на синхронизиране.</span><span class="sxs-lookup"><span data-stu-id="f6180-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="f6180-104">Преинсталирането на AADConnect с помощта на експресни настройки може да реши проблема бързо:</span><span class="sxs-lookup"><span data-stu-id="f6180-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="f6180-105">[Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="f6180-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="f6180-106">[Следвайте инструкциите за експресна инсталация](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="f6180-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="f6180-107">Azure AD Connect трябва да се инсталира на Windows Server 2012 или по-нова версия.</span><span class="sxs-lookup"><span data-stu-id="f6180-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="f6180-108">Този сървър трябва да бъде присъединен към домейн и може да бъде домейнов контролер или сървър член.</span><span class="sxs-lookup"><span data-stu-id="f6180-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="f6180-109">За пълен списък на изискванията за Свързване и предварителните изисквания на Azure AD прегледайте Предварителни [изисквания за Azure AD Свързване.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="f6180-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="f6180-110">За повече информация относно акаунтите за услуги на AADConnect вж. [Azure AD Свързване: Акаунти и разрешения.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="f6180-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
