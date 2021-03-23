---
title: Отстраняване на неизправности с еднократната идентификация за Azure AD присъединен устройства
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034925"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="945d0-102">Отстраняване на неизправности с еднократната идентификация за Azure AD присъединен устройства</span><span class="sxs-lookup"><span data-stu-id="945d0-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="945d0-103">Ако имате локална среда за Active Directory (AD) и искате да се присъедините към своя РЕКЛАМен домейн, към който се присъединяват компютрите към Azure AD, можете да постигнете това, като направите хибридно Azure AD съединение.</span><span class="sxs-lookup"><span data-stu-id="945d0-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="945d0-104">[Как да: планиране Вашият хибриден Azure Active Directory присъединяване към приложението](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ви предоставя свързаните стъпки за реализиране на хибридна Azure ad съединение във вашата среда.</span><span class="sxs-lookup"><span data-stu-id="945d0-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="945d0-105">За повече информация вижте [Конфигуриране на устройства, свързани с AZURE ad, за локални Single-Sign за използване на Windows Hello за бизнеса](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="945d0-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="945d0-106">**Проблеми в основния маркер за обновяване (PRT)**</span><span class="sxs-lookup"><span data-stu-id="945d0-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="945d0-107">Маркерът за първичен обновяване (PRT) е ключов артефакт на Azure AD удостоверяване в Windows 10, Windows Server 2016 и по-нови версии, устройства с iOS и Android.</span><span class="sxs-lookup"><span data-stu-id="945d0-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="945d0-108">Това е JSON уеб маркер (JWT), специално издадено на брокери на Microsoft First-токен, за да се разреши еднократната идентификация (SSO) между приложенията, използвани за тези устройства.</span><span class="sxs-lookup"><span data-stu-id="945d0-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="945d0-109">За подробности относно начина, по който даден PRT е издаден, използван и защитен на устройства с Windows 10, вижте [Какво е първичен маркер за обновяване?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="945d0-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="945d0-110">**WamDefaultSet: да и AzureADPrt: да**</span><span class="sxs-lookup"><span data-stu-id="945d0-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="945d0-111">Тези полета указват дали потребителят е удостоверен успешно в Azure AD при влизане в устройството.</span><span class="sxs-lookup"><span data-stu-id="945d0-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="945d0-112">Ако стойностите са " **не**", това може да се дължи на:</span><span class="sxs-lookup"><span data-stu-id="945d0-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="945d0-113">Грешен ключ за място за съхранение в TPM, асоцииран с устройството при регистрацията (проверка на KeySignTest при работа с повишени стойности)</span><span class="sxs-lookup"><span data-stu-id="945d0-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="945d0-114">Алтернативен ИД за влизане</span><span class="sxs-lookup"><span data-stu-id="945d0-114">Alternate Login ID</span></span>
- <span data-ttu-id="945d0-115">Не е намерен HTTP прокси сървър</span><span class="sxs-lookup"><span data-stu-id="945d0-115">HTTP Proxy not found</span></span>

<span data-ttu-id="945d0-116">За отстраняване на неизправности при устройства с помощта на командата dsregcmd вижте [SSO](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="945d0-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
