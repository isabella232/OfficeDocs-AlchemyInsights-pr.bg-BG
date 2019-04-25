---
title: 646 как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399760"
---
# <a name="configure-sync-features"></a><span data-ttu-id="6bee2-102">Конфигуриране на функции в синхронизиране</span><span class="sxs-lookup"><span data-stu-id="6bee2-102">Configure sync features</span></span>

<span data-ttu-id="6bee2-103">Лазурно АД свързване включва няколко функции, които са разрешени по подразбиране, или че можете да активирате по-късно.</span><span class="sxs-lookup"><span data-stu-id="6bee2-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="6bee2-104">Някои функции изискват допълнителна конфигурация в специфични среди.</span><span class="sxs-lookup"><span data-stu-id="6bee2-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="6bee2-105">[Филтрирането](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) граници обектите се синхронизират в лазурно АД.</span><span class="sxs-lookup"><span data-stu-id="6bee2-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="6bee2-106">По подразбиране, всички потребители, контакти, групи и Windows 10 Компютърни акаунти са синхронизирани.</span><span class="sxs-lookup"><span data-stu-id="6bee2-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="6bee2-107">Можете да включват или изключват обекти, базирани на домейни, OU или други атрибути.</span><span class="sxs-lookup"><span data-stu-id="6bee2-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="6bee2-108">[Парола кълцам цикличният](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизирам определителен член парола кълцам от локалната Active Directory към лазурните реклама.</span><span class="sxs-lookup"><span data-stu-id="6bee2-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="6bee2-109">Това позволява управление на парола в едно място, но използването на една и съща парола в двете локални и облак среди.</span><span class="sxs-lookup"><span data-stu-id="6bee2-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="6bee2-110">Тъй като Active Directory е достоверният източник, можете да използвате своя собствена парола политика.</span><span class="sxs-lookup"><span data-stu-id="6bee2-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="6bee2-111">[Самообслужване парола проучване (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да сменят паролите си собствени в облака, докато все още се прилага вашата локалната парола политика.</span><span class="sxs-lookup"><span data-stu-id="6bee2-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="6bee2-112">[Writeback определителен устройство](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява регистрирани устройства в лазурно Рекламата да се запише обратно в локалната Active Directory, така че те могат да бъдат използвани за условен достъп.</span><span class="sxs-lookup"><span data-stu-id="6bee2-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="6bee2-113">[Предотвратяване на случайно изтриване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е активирана по подразбиране за да се предотврати прекалено много едновременни обект делеции (повече от 500 обекта за синхронизация).</span><span class="sxs-lookup"><span data-stu-id="6bee2-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="6bee2-114">Можете да промените тази настройка, за да отговори на нуждите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="6bee2-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="6bee2-115">[Автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е активирана по подразбиране за Експресно инсталации и помага да се гарантира вашата версия на Azure АД свържете е винаги актуална.</span><span class="sxs-lookup"><span data-stu-id="6bee2-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
