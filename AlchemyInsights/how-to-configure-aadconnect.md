---
title: 646 Как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722516"
---
# <a name="configure-sync-features"></a><span data-ttu-id="7041d-102">Конфигуриране на функциите за синхронизиране</span><span class="sxs-lookup"><span data-stu-id="7041d-102">Configure sync features</span></span>

<span data-ttu-id="7041d-103">Azure AD свързване включва няколко функции, които са разрешени по подразбиране или можете да разрешите по-късно.</span><span class="sxs-lookup"><span data-stu-id="7041d-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="7041d-104">Някои функции изискват допълнителна конфигурация в определени среди.</span><span class="sxs-lookup"><span data-stu-id="7041d-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="7041d-105">[Филтриране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) граници обекти са синхронизирани Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7041d-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="7041d-106">По подразбиране се синхронизират всички потребители, контакти, групи и акаунти на компютъра в Windows 10.</span><span class="sxs-lookup"><span data-stu-id="7041d-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="7041d-107">Можете да включите или изключите обекти на базата на домейни, ous или други атрибути.</span><span class="sxs-lookup"><span data-stu-id="7041d-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="7041d-108">[Парола хеш синхронизация](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизира паролата хеш от локалната Active Directory azure AD.</span><span class="sxs-lookup"><span data-stu-id="7041d-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="7041d-109">Това позволява управление на пароли на едно място, но използването на една и съща парола както в локалните, така и в облачните среди.</span><span class="sxs-lookup"><span data-stu-id="7041d-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="7041d-110">Тъй като Active Directory е авторитетен източник, можете да използвате вашите собствени правила за парола.</span><span class="sxs-lookup"><span data-stu-id="7041d-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="7041d-111">[Самостоятелно нулиране на паролата (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да нулират собствените си пароли в облака, като все още прилагат правилата за локална парола.</span><span class="sxs-lookup"><span data-stu-id="7041d-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="7041d-112">[Устройство с отпиване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява регистрирани те да бъдат записани в Azure AD да бъдат записани обратно в локалната Active Directory, така че те могат да се използват за условен достъп.</span><span class="sxs-lookup"><span data-stu-id="7041d-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="7041d-113">[Предотвратяване на случайни изтривания](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е разрешена по подразбиране да предотврати твърде много едновременни обекти изтривания (повече от 500 обекти за синхронизация).</span><span class="sxs-lookup"><span data-stu-id="7041d-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="7041d-114">Можете да промените тази настройка, за да отговаря на нуждите на вашата организация.</span><span class="sxs-lookup"><span data-stu-id="7041d-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="7041d-115">[Автоматичното надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е активирано по подразбиране за експресни инсталации и помага да се гарантира, че вашата версия на Azure AD Connect е винаги актуална.</span><span class="sxs-lookup"><span data-stu-id="7041d-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
