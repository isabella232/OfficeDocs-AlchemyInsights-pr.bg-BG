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
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986880"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Коригиране на Microsoft 365 "Модулът за надеждна платформа на вашия компютър не работи правилно"

За да коригирате грешката, използвайте стъпките по-долу:

- Инсталирайте най-новите [актуализации за Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Опитайте процеса [на възстановяване на потребителите,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) за да коригирате грешките в модула за надеждна платформа (TPM).
- Задайте EnableADAL = 0, като използвате следните стъпки:  
    1. Щракнете с десния бутон върху бутона Windows "Старт", **изберете Изпълнение**, **въведете regedit** и след това изберете **OK**.
    2. Изберете **Да,** за да позволите на редактора на системния регистър да прави промени във вашето устройство.
    3. В редактора на системния регистър добавете DWORD стойност на **EnableADAL** с настройка **0** под HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

За повече информация вижте Проблеми с връзката при влизане след [актуализация до Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).