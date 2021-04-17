---
title: Противодействие на грешка Приложението не е открито
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836340"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="f8347-102">Противодействие на грешка "Приложението не е открито"</span><span class="sxs-lookup"><span data-stu-id="f8347-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="f8347-103">Грешката при инсталиране на приложението, "Приложението не е открито след успешното завършване на инсталацията", съобщено от Intune, може да възникне на всички основни операционни системи (Windows, iOS и Android).</span><span class="sxs-lookup"><span data-stu-id="f8347-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="f8347-104">Най-често срещаните сценарии за генериране на тази грешка са:</span><span class="sxs-lookup"><span data-stu-id="f8347-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="f8347-105">Приложението е актуализирано извън Intune (от магазин за приложения на други разработчици) след първоначалното разполагане.</span><span class="sxs-lookup"><span data-stu-id="f8347-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="f8347-106">Например някои приложения, като напр. Google Chrome, може да извършват автоматични актуализации.</span><span class="sxs-lookup"><span data-stu-id="f8347-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="f8347-107">Потребител е деинсталирал приложението след първоначалното инсталиране.</span><span class="sxs-lookup"><span data-stu-id="f8347-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="f8347-108">За да противодействате на този проблем, първо трябва да извършите преглед на засегнатите устройства, за да определите сценария, в който е възникнала грешката.</span><span class="sxs-lookup"><span data-stu-id="f8347-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="f8347-109">Ако приложението е актуализирано извън Intune, разполагането на приложението може да бъде настроено да игнорира версията на приложението.</span><span class="sxs-lookup"><span data-stu-id="f8347-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="f8347-110">За да направите това, под **Конфигуриране на приложението > Информация за приложението** задайте версията **Игнориране на приложението** на **Да**.</span><span class="sxs-lookup"><span data-stu-id="f8347-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="f8347-111">При насочване към клиента може да е подходящо да разположите приложението като "задължително" и да се уверите, че най-новата версия е разположена.</span><span class="sxs-lookup"><span data-stu-id="f8347-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="f8347-112">Алтернативно, на платформата iOS е възможно да използвате функцията **автоматичното актуализиране**, свързана с програмата за закупуване на томове на Apple, която може да бъде конфигурирана да се актуализира автоматично до новите версии на приложенията, когато бъдат налични.</span><span class="sxs-lookup"><span data-stu-id="f8347-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="f8347-113">За повече информация за отстраняването на неизправности при инсталиране на приложението вж. [Отстраняване на проблеми при инсталирането на приложения](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="f8347-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
