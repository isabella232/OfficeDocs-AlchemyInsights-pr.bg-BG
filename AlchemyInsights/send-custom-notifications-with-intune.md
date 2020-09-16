---
title: Изпращане на персонализирани уведомления чрез настройка
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720635"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="afb3e-102">Как се изпращат персонализирани уведомления за потребителите на управлявани устройства с iOS и Android</span><span class="sxs-lookup"><span data-stu-id="afb3e-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="afb3e-103">Персонализираните уведомления за настройка се обработват от приложението Company Portal на устройство на потребител.</span><span class="sxs-lookup"><span data-stu-id="afb3e-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="afb3e-104">След това приложението създава Push известието на това устройство.</span><span class="sxs-lookup"><span data-stu-id="afb3e-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="afb3e-105">По-долу ще намерите предварителни изисквания за устройството, за да поддържате получаването на известия по избор, и за приложението, след което ще създадете Push известието:</span><span class="sxs-lookup"><span data-stu-id="afb3e-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="afb3e-106">Устройството трябва да е инсталирано приложението Company Portal.</span><span class="sxs-lookup"><span data-stu-id="afb3e-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="afb3e-107">Устройството трябва да позволява на приложението "фирмен портал" да изпраща насочени известявания.</span><span class="sxs-lookup"><span data-stu-id="afb3e-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="afb3e-108">Когато приложението се инсталира или актуализира, той ще подкани потребителя да разреши уведомленията.</span><span class="sxs-lookup"><span data-stu-id="afb3e-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="afb3e-109">Устройства с Android трябва да имат инсталирани услуги на Google Play.</span><span class="sxs-lookup"><span data-stu-id="afb3e-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="afb3e-110">Устройството трябва да е записано с "включено".</span><span class="sxs-lookup"><span data-stu-id="afb3e-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="afb3e-111">За повече информация как да изпратите съобщение вижте [документацията за функции](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="afb3e-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
