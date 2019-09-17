---
title: Изпращане на персонализирани известия с InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992302"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a145f-102">Как да изпратите персонализирани уведомления на потребителите на управлявани iOS и Android устройства</span><span class="sxs-lookup"><span data-stu-id="a145f-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a145f-103">Персонализираните известия за InTune се обработват от приложението на портала на компанията на устройството на потребителя.</span><span class="sxs-lookup"><span data-stu-id="a145f-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a145f-104">След това приложението създава Push известието на това устройство.</span><span class="sxs-lookup"><span data-stu-id="a145f-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a145f-105">По-долу са предпоставки за устройство за поддръжка на получаване на потребителски известия и приложението да създадете Push уведомление:</span><span class="sxs-lookup"><span data-stu-id="a145f-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a145f-106">Устройството трябва да има инсталирано приложението Company Portal.</span><span class="sxs-lookup"><span data-stu-id="a145f-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a145f-107">Устройството трябва да позволи на приложението на портала на компанията да изпраща известия за Push.</span><span class="sxs-lookup"><span data-stu-id="a145f-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a145f-108">Когато приложението е инсталирано или актуализирано, то ще подкани потребителя да разреши известията.</span><span class="sxs-lookup"><span data-stu-id="a145f-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a145f-109">Устройствата с Android трябва да имат инсталирани услуги на Google Play.</span><span class="sxs-lookup"><span data-stu-id="a145f-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a145f-110">Устройството трябва да бъде записано с InTune.</span><span class="sxs-lookup"><span data-stu-id="a145f-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a145f-111">За повече информация, включително как да изпратите съобщение, вижте [документацията на функцията](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="a145f-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
