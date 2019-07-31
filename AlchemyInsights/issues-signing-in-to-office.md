---
title: Проблеми с влизане в офис приложения
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938135"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Празен екран за вход в офис приложения

За да коригирате този проблем, опитайте следното:
- Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Начално състояние на Internet Explorer опции: отидете в **инструменти** > **Интернет опции** > **Разширени** > **Нулиране на настройките на Internet Explorer** (имайте предвид, че ще загубите персонализирани настройки) и след това се опитайте влизате отново в офиса.
- Да изключите Windows Defender приложение охрана (WDAG) или друга подобна защитна стена или антивирусна програма:
    1. В контролния панел преминете към **програми**и след това изберете **въртя Прозорец черта на или на разстояние**.
    2. Ако Windows Defender приложение гвардия е разрешено, опитайте да го забраните.<br/>
    **Забележка:** Може да се наложи да рестартирате компютъра.
- Уверете се, че Microsoft.AAD.BrokerPlugin [Пад WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) не е блокиран от всяко приложение или програма за защитна стена и антивирусен.
- [Ясно Office идентификационни данни](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощта на диспечера на идентификационни данни на Windows.<br/>
    **Забележка:** Регистър пътеки за Office 2016 са се променили до 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

За повече информация вижте [връзката проблеми в вход след актуализация на Office 2016 строя 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).