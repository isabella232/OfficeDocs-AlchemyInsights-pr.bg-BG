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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695168"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Поправянето на приложенията на Microsoft 365 "съобщение за надеждна платформа на компютъра ви не функционира правилно"

За да коригирате грешката, използвайте стъпките по-долу:

- Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ех: \Software\Microsoft\Office\16.0\Common\Identity\)
- Изпробвайте [процеса за възстановяване на потребител](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) , за да поправите грешките в модула за надеждна платформа (TPM).
- Задайте или enableadal = 0 с помощта на следните стъпки:  
    1. Щракнете с десния бутон върху бутона "Старт" на Windows, изберете **изпълнение**, въведете **regedit**и след това изберете **OK**.
    2. Изберете **да** , за да разрешите на редактора на системния регистър да прави промени на вашето устройство.
    3. В редактора на системния регистър Добавете DWORD стойност на **или enableadal** с настройка **0** под HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

За повече информация вижте [проблеми с връзката при влизане, след като сте актуализирали до Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).