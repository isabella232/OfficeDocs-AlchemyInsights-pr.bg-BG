---
title: Проблеми при влизане в приложения на Microsoft 365
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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833020"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Празен екран за влизане в приложенията на Microsoft 365

За да коригирате този проблем, опитайте следното:
- Инсталирайте най-новите актуализации [за Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Нулиране на опциите на Internet Explorer: Отидете на Инструменти Internet  >  **Options**  >  **Advanced**  >  **Reset Internet Explorer Settings** (имайте предвид, че ще загубите настройките по избор) и след това опитайте да влезете отново в Office.
- Забраняване на Windows Defender Application Guard (WDAG) или подобна защитна стена или антивирусна програма:
    1. В контролния панел отидете на **Програми и** след това изберете Включване или изключване **на функциите на Windows.**
    2. Ако Windows Defender Application Guard е разрешен, опитайте да го изключите.<br/>
    **Забележка:** Може да се наложи да рестартирате компютъра.
- Уверете се, че добавката Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не се блокира от приложение или защитна стена/антивирусна програма.
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

За повече информация вижте Проблеми с връзката при влизане след актуализация до [компилация на Office 2016 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).