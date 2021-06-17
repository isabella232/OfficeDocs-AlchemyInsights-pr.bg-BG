---
title: Използване на Microsoft Intune за управление на уеб достъпа в Microsoft Edge за iOS и Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989646"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="f6afd-102">Използване на Microsoft Intune за управление на уеб достъпа в Microsoft Edge за iOS и Android</span><span class="sxs-lookup"><span data-stu-id="f6afd-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="f6afd-103">Microsoft Edge за iOS и Android позволява на потребител да преглежда уеб от множество, напълно отделни профили.</span><span class="sxs-lookup"><span data-stu-id="f6afd-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="f6afd-104">Най-широките възможности за защита за данни на Microsoft 365 стават достъпни, когато се абонирате за пакета Enterprise Mobility + Security, който включва функциите Microsoft Intune и Azure Active Directory Premium, като например условен достъп.</span><span class="sxs-lookup"><span data-stu-id="f6afd-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="f6afd-105">Най-малко ще искате да разположите правила за условен достъп, които (1) позволяват на потребителите да се свързват от мобилни устройства към Microsoft Edge за iOS и Android и че (2) прилага правила за защита на приложения на Microsoft Intune, които предоставят защитена среда за сърфиране.</span><span class="sxs-lookup"><span data-stu-id="f6afd-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="f6afd-106">За да разберете как можете да използвате условен достъп и правила, вижте:</span><span class="sxs-lookup"><span data-stu-id="f6afd-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="f6afd-107">Прилагане на правила за условен достъп на Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="f6afd-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="f6afd-108">Създаване на правила за защита на приложения на Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f6afd-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="f6afd-109">Използване на еднократната регистрация за уеб приложения, свързани с Azure Active Directory, в защитени с правила браузъри</span><span class="sxs-lookup"><span data-stu-id="f6afd-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="f6afd-110">Използване на конфигурацията на приложението за управление на работата при сърфиране</span><span class="sxs-lookup"><span data-stu-id="f6afd-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="f6afd-111">Разрешаване на използването само на акаунти за работа и училище</span><span class="sxs-lookup"><span data-stu-id="f6afd-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="f6afd-112">Разполагане на общи правила за конфигуриране на приложения</span><span class="sxs-lookup"><span data-stu-id="f6afd-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="f6afd-113">Разполагане на правила за конфигуриране на приложения за защита на данните</span><span class="sxs-lookup"><span data-stu-id="f6afd-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="f6afd-114">Използване на Microsoft Endpoint Manager за разполагане на правила за конфигуриране на приложения</span><span class="sxs-lookup"><span data-stu-id="f6afd-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="f6afd-115">За да научите как да получите достъп до регистрационните файлове на управлявани приложения, вижте Използване на [Microsoft Edge за iOS и Android за достъп до регистрационните файлове на управлявани приложения.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="f6afd-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
