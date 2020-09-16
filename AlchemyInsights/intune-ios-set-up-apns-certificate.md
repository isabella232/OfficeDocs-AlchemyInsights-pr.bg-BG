---
title: Настройване на APN сертификат с Intune за iOS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: f58405de018c916e08672022bb4f66292524b736
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667435"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="4cd22-102">Настройване на APN сертификат с Intune за iOS</span><span class="sxs-lookup"><span data-stu-id="4cd22-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="4cd22-103">Сертификат за Apple MDM Push (наричана още "услуга за насочени известия на Apple), - APN сертификат - не е конфигуриран за абонамента ви.</span><span class="sxs-lookup"><span data-stu-id="4cd22-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="4cd22-104">Без конфигуриран сертификат Apple MDM Push не можете да се записвате и да управлявате устройства с iOS и MacOS.</span><span class="sxs-lookup"><span data-stu-id="4cd22-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="4cd22-105">След като добавите сертификата в Intune, вашите потребители ще могат да инсталират приложението Company Portal, за да се записват от своите устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="4cd22-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="4cd22-106">За ръководство "стъпка по стъпка" за добавяне на APN сертификат към вашия клиент за Intune, прегледайте съдържанието на следния линк:</span><span class="sxs-lookup"><span data-stu-id="4cd22-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="4cd22-107">Получете сертификат на Apple MDM Push</span><span class="sxs-lookup"><span data-stu-id="4cd22-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="4cd22-108">Ако имате проблеми със сертификата за насочени известия на Apple (APNS), вижте тази публикация в блог: [Intune и APN сертификат: често задавани въпроси и общи проблеми](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="4cd22-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
