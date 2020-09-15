---
title: 646 как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704478"
---
# <a name="configure-sync-features"></a><span data-ttu-id="bc9fd-102">Конфигуриране на функции за синхронизиране</span><span class="sxs-lookup"><span data-stu-id="bc9fd-102">Configure sync features</span></span>

<span data-ttu-id="bc9fd-103">Azure AD Connect включва няколко функции, които са разрешени по подразбиране, или че можете да ги разрешите по-късно.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="bc9fd-104">Някои функции изискват допълнителна конфигурация в определени среди.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="bc9fd-105">Ограничения за [филтриране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обектите се синхронизират с Azure ad.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="bc9fd-106">По подразбиране всички потребители, контакти, групи и акаунти за компютри с Windows 10 се синхронизират.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="bc9fd-107">Можете да включвате или изключвате обекти на базата на домейни, OU или други атрибути.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="bc9fd-108">[Синхронизиране на хеширане на парола](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизира Хеширането на парола от локалния указател Active Directory в Azure ad.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="bc9fd-109">Това позволява управление на паролите на едно място, но използва същата парола както в локалната среда, така и в облака.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="bc9fd-110">Тъй като Active Directory е авторитетен източник, можете да използвате собствените си правила за парола.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="bc9fd-111">[Услугата за самостоятелно нулиране на парола (парола)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да нулират своите собствени пароли в облака, като все пак прилагат вашите локални правила за парола.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="bc9fd-112">[Device нефиксирани](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява на регистрираните устройства в Azure ad да се изписват обратно в локалния указател Active Directory, така че да могат да бъдат използвани за условен достъп.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="bc9fd-113">[Предотвратяване на случайни изтривания](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е разрешено по подразбиране, за да се предотврати твърде много изтривания на едновременни обекти (повече от обекти на 500 за синхронизация).</span><span class="sxs-lookup"><span data-stu-id="bc9fd-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="bc9fd-114">Можете да промените тази настройка така, че да отговаря на нуждите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="bc9fd-115">[Автоматичната надстройка](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е разрешена по подразбиране за експресните инсталации и помага да се гарантира, че вашата версия на Azure ad Connect винаги е актуална.</span><span class="sxs-lookup"><span data-stu-id="bc9fd-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
