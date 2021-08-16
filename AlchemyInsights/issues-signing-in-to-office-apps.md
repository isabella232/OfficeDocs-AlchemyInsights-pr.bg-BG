---
title: Проблеми при влизане в Microsoft 365 приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028029"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Коригиране на Microsoft 365 "За съжаление, вече е влезли друг акаунт от вашата организация"

За да коригирате грешката, използвайте стъпките по-долу:

- Премахнете всички работни акаунти, с изключение на засегнатия акаунт, като използвате Windows Настройки > **access work или school**.
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Отворете приложение Office, изберете **Излизане от**  >    >  **файлов акаунт**. След това влезте с помощта на потребителски акаунт с валиден лиценз. За подробна информация вж. [Акаунти в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- За Mac вж. [Не можете да влезете в приложение на Office 2016 за Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

За повече информация вижте "За съжаление, друг акаунт от вашата организация вече е влезли на [този компютър" в Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)