---
title: Проблеми при влизане в приложения на Microsoft 365
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
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579854"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Коригиране на Microsoft 365 приложения "модулът на надеждната платформа на компютъра не функционира правилно"

За да коригирате грешката, използвайте стъпките по-долу:

- Инсталирайте най-новите актуализации за [Windows](https://support.microsoft.com/help/4027667/windows-10-update) и [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Изчистване на идентификационни данни за Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) чрез диспечера за идентификационни данни на Windows.<br/>
    **Забележка:** Пътищата от системния регистър за Office 2016 са променени на 16.0. (Напр:\софтуер\Microsoft\Office\16.0\Common\Identity\)
- Опитайте [процеса](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) на възстановяване на потребителя да поправи грешките на модула за надеждна платформа (TPM).
- Задайте EnableADAL = 0, като използвате следните стъпки:  
    1. Щракнете с десния бутон върху бутона "Старт" на Windows, изберете **Изпълнение**, въведете **regedit**, след което изберете **OK**.
    2. Изберете **Да,** за да позволите на редактора на системния регистър да прави промени в устройството ви.
    3. В редактора на системния регистър добавете DWORD стойност на **EnableADAL** с настройка **0** под HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

За повече информация вижте [проблеми с връзката след актуализация за Office 2016 компилация 16.0.7967 на Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).