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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695276"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Празен екран за влизане в приложенията на Microsoft 365

За да коригирате този проблем, опитайте следното:
- Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Нулиране на опциите **за Internet Explorer: отидете на**  >  **Опции за интернет**за  >  **Разширени**  >  **нулиране на настройките на Internet Explorer** (обърнете внимание, че ще загубите потребителските настройки) и след това опитайте да влезете отново в Office.
- Забраняване на приложението за защита на приложения на Windows Defender (WDAG) или подобна защитна стена или антивирусна програма:
    1. В контролния панел отидете на **програми**и след това изберете **включване и изключване на функции на Windows**.
    2. Ако е разрешена защитата на приложения на Windows Defender, опитайте да я забраните.<br/>
    **Забележка:** Може да се наложи да рестартирате компютъра.
- Уверете се, че добавката Microsoft. пад. BrokerPlugin [в пад за матуритет](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не се блокира от никое приложение или защитна стена/антивирусна програма.
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ех: \Software\Microsoft\Office\16.0\Common\Identity\)

За повече информация вижте [проблеми с връзката при влизане, след като сте актуализирали до Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).