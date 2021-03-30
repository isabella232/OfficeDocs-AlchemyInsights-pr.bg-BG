---
title: Single-Sign за устройства, присъединени към Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404247"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="fbaec-102">Еднократна регистрация за устройства, присъединени към Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fbaec-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="fbaec-103">Ако имате локална среда на Active Directory (AD) и искате да се присъедините към компютрите си, присъединени към домейна на AD, към Azure AD, можете да постигнете това, като направите хибридно присъединяване към Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fbaec-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="fbaec-104">[Как да: Планирането на вашата хибридна реализация на присъединяване към Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за внедряване на хибридно присъединяване на Azure AD във вашата среда.</span><span class="sxs-lookup"><span data-stu-id="fbaec-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="fbaec-105">Конфигуриране на устройства, присъединени към Azure AD, за локални Single-Sign При използване на Windows Hello за бизнеса</span><span class="sxs-lookup"><span data-stu-id="fbaec-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="fbaec-106">**Проблеми с маркера за основно обновяване (PRT)** Маркерът за основно обновяване (PRT) е ключов артефакт на удостоверяването на Azure AD на устройства с Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="fbaec-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="fbaec-107">Това е JSON Web Token (JWT), специално издаден на брокери на маркери на Microsoft от първа страна, за да разрешите еднократната регистрация (SSO) в приложенията, използвани на тези устройства.</span><span class="sxs-lookup"><span data-stu-id="fbaec-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="fbaec-108">[В Какво представлява маркерът за](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)основно обновяване? ще ви предоставим подробности как се издава, използва и защитава PRT на устройства с Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fbaec-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="fbaec-109">**WamDefaultSet: YES и AzureADPrt: YES** Тези полета показват дали потребителят е удостоверен успешно с Azure AD при влизане в устройството.</span><span class="sxs-lookup"><span data-stu-id="fbaec-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="fbaec-110">Ако стойностите са **НЕ,** може да е дължимо:</span><span class="sxs-lookup"><span data-stu-id="fbaec-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="fbaec-111">Лош ключ за съхранение в TPM, свързан с устройството при регистрация (проверете KeySignTest, докато се изпълнява повишени).</span><span class="sxs-lookup"><span data-stu-id="fbaec-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="fbaec-112">Алтернативен ИД на влизане</span><span class="sxs-lookup"><span data-stu-id="fbaec-112">Alternate Login ID</span></span>
- <span data-ttu-id="fbaec-113">HTTP прокси сървърът не е намерен</span><span class="sxs-lookup"><span data-stu-id="fbaec-113">HTTP Proxy not found</span></span>

<span data-ttu-id="fbaec-114">Отстраняване на неизправности с устройства с помощта на командата dsregcmd – [състояние на SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="fbaec-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
