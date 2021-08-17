---
title: Приложение за удостоверяване
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
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082931"
---
# <a name="authentication-app"></a>Приложение за удостоверяване

Ако сте глобален администратор, можете бързо да разберете какво се е случило или да диагностицирате проблеми, свързани с влизането на потребителя, с помощта [на диагностиката за влизане.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Стартирайте диагностиката, като щракнете върху бутона["Стартиране на](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)диагностиката". 
1. Намерете събитието, за да анализирате, като въведете подробните данни за потребителя, приложението, часа на влизане, ИД на заявка или ИД на корелация.
1. Прегледайте диагностичните резултати, показващи подробностите за случилото се и какви действия можете да предприемете, за да направите промени, ако са необходими някакви промени.

**Проверете сценария, който е приложим:**

1. Ако потребителят не получава push известие в приложението Microsoft Authenticator, проверете дали не се показват под блокираните потребители на MFA, както е описано в [Блокиране и разблокиране на потребители.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ако потребителят не е блокиран за MFA, но не получи push известие, той може да отвори приложението Microsoft Authenticator, което ще изтегли чакащите искания за одобрение.
1. Като алтернативен метод за влизане потребителят може също да щракне върху Влизане по друг начин и да избере да използва код за потвърждение от мобилното ми приложение.
1. Приложението Microsoft Authenticator е единственият наличен метод за много потребители. [Научете повече за настройките по подразбиране за](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)защита, Authenticator [често](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) задавани въпроси за приложението за често задавани въпроси и как да ги разрешите.
 
**Препоръчителни видеоклипове**

[Как да настроите Authenticator на нов телефон (2 минути).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
