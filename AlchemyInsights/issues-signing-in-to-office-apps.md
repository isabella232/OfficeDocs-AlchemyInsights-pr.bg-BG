---
title: Проблеми при влизане в приложенията на Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695312"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Коригиране на приложенията на Microsoft 365 "за съжаление, друг акаунт от вашата организация вече е влязъл" съобщение

За да коригирате грешката, използвайте стъпките по-долу:

- Премахнете всички служебни акаунти, с изключение на засегнатия акаунт, с помощта на настройките на Windows > **Access Work или School**.
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ех: \Software\Microsoft\Office\16.0\Common\Identity\)
- Отворете приложение на Office, изберете **File**  >  **Account**  >  **излизане от**акаунт за файл. След това влезте с потребителски акаунт с валиден лиценз. За подробна информация вж. [Акаунти в Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- За Mac вж. [Не можете да влезете в приложение на Office 2016 за Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

За повече информация вижте ["за съжаление, друг акаунт от вашата организация вече е влязъл на този компютър" в Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).