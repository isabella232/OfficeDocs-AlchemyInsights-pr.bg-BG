---
title: Проблеми при влизане в приложения
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900763"
---
# <a name="issues-signing-in-to-applications"></a>Проблеми при влизане в приложения

За откриване на проблемите с причината или диагностицирането, свързани с потребителското влизане, изпълнете следните стъпки:

1. Стартирайте [диагностичната диагностика за влизане](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Намерете събитието, което искате да анализирате чрез въвеждане на данните, които имате за потребителя, приложението, часа на влизане, ИД на заявка или ИД на корелация.
3. Прегледайте диагностичните резултати, които показват подробностите за това какво се е случило и какви действия можете да предприемете, за да направите промени, ако са необходими промени.

По-долу са описани някои често срещани проблеми при влизане в приложения:

1. Вие или потребителят сте **завършили влизане в AZURE ad, но виждате неочаквана подкана** да видите статиите за [неочаквано съгласие при влизане в приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) и [неочаквана грешка при извършване на съгласие за приложение](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Вие или потребител сте **влезли директно в дадено приложение, но не можете да влезете в него от deeplink в портала по избор или панела на Access**: Вижте отстраняване на [проблеми при влизане в приложение от Azure ad my Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Вие или потребител сте **завършили влизане в AZURE ad, но приложението показва съобщение за грешка и не позволява на потребителя да завърши потока за влизане**: Проблемът е, че приложението не приема отговора, издаден от Azure ad. Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) , за да отстраните проблема.
4. Вие или потребител **не можете да влезете в приложение, което не е в галерия, което е конфигурирано за еднократна идентификация на парола**: Следвайте указанията в [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) за отстраняване на неизправности.
5. Вие или потребител **не можете да влезете в приложение на AZURE ad Gallery, конфигурирано за еднократна идентификация на парола**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , за да отстраните проблема.
6. Потребителят **не може да влезе в приложение на Microsoft**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) , за да отстраните проблема.
7. Вие или потребител **не можете да влезете в приложение, което не е в галерия, конфигурирано за външни единични записвания**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) , за да отстраните проблема.
8. Вие или потребител **не можете да влезете в приложение на AZURE ad Gallery, конфигурирано за външни единични записвания**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , за да отстраните проблема.
9. Потребителят **не може да влезе в приложение, което е разработен по избор**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , за да отстраните проблема.
10. Потребителят **не може да влезе в локално приложение с помощта на прокси сървъра за приложения на AZURE ad**: Следвайте [тези стъпки](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) , за да отстраните проблема.

