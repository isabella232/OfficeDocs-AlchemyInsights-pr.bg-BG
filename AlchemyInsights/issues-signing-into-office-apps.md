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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938136"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Определяне на Office приложения "на вашия компютър опекун платформа модулирам е не функционира правилно" съобщението

За да коригирате тази грешка, опитайте следното:

- Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Ясно Office идентификационни данни](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) с помощта на диспечера на идентификационни данни на Windows.<br/>
    **Забележка:** Регистър пътеки за Office 2016 са се променили до 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Опитайте на [потребителя възстановяване процес](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) към прикрепвам модул за надеждна платформа (TPM) повреди.
- Задайте EnableADAL = 0, използвайки следните стъпки:  
    1. С десния бутон върху бутона Старт на Windows, изберете **изпълнение**, въведете **regedit**и след това изберете **OK**.
    2. Изберете **"да"** да се даде възможност на редактора на системния регистър да направите промени в устройството.
    3. В редактора на системния регистър Добавете DWORD стойност на **EnableADAL** с настройка на **0** под HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

За повече информация вижте [връзката проблеми в вход след актуализация на Office 2016 строя 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).