---
title: Настройване на APN сертификат с Intune за iOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824028"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="7ca1f-102">Настройване на APN сертификат с Intune за iOS</span><span class="sxs-lookup"><span data-stu-id="7ca1f-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="7ca1f-103">Сертификат за Apple MDM Push (наричана още "услуга за насочени известия на Apple), - APN сертификат - не е конфигуриран за абонамента ви.</span><span class="sxs-lookup"><span data-stu-id="7ca1f-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="7ca1f-104">Без конфигуриран сертификат Apple MDM Push не можете да се записвате и да управлявате устройства с iOS и MacOS.</span><span class="sxs-lookup"><span data-stu-id="7ca1f-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="7ca1f-105">След като добавите сертификата в Intune, вашите потребители ще могат да инсталират приложението Company Portal, за да се записват от своите устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="7ca1f-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="7ca1f-106">За ръководство "стъпка по стъпка" за добавяне на APN сертификат към вашия клиент за Intune, прегледайте съдържанието на следния линк:</span><span class="sxs-lookup"><span data-stu-id="7ca1f-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="7ca1f-107">Получете сертификат на Apple MDM Push</span><span class="sxs-lookup"><span data-stu-id="7ca1f-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="7ca1f-108">Ако имате проблеми със сертификата за насочени известия на Apple (APNS), вижте тази публикация в блог: [Intune и APN сертификат: често задавани въпроси и общи проблеми](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="7ca1f-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
