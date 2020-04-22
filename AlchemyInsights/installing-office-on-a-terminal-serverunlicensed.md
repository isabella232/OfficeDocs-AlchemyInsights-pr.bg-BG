---
title: Инсталиране на офис на терминален сървър - нелицензиран
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763206"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране на Office на терминален сървър

За разполагане на Приложения на Microsoft 365 за предприятие на Windows Server с помощта на услуги за отдалечен работен плот (RDS), наричани преди терминални услуги:
  
- Трябва да имате абонамент за Microsoft 365, който включва приложения на Microsoft 365 за предприятие, като например Office 365 Enterprise E3 или Enterprise E5. Microsoft 365 приложения за бизнес и Приложения на Microsoft 365 за бизнес планове Premium не включват приложения на Microsoft 365 за предприятие.

- Трябва да разрешите [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ако искате да инсталирате Приложения на Microsoft 365 за предприятие на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране,*** използвайте следните стъпки.

> [!TIP]
> Можете също да изтеглите и стартирате поддръжката на [Microsoft и помощника](https://aka.ms/SaRA_OfficeSCA_M365Portal) за възстановяване, за да инсталирате Приложения на Microsoft 365 за предприятие в режим на активиране на споделен компютър.
  
1. Проверете какво абонамент за Microsoft 365 имате. [Научете как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, преминете към друг абонамент за Microsoft 365. [Научете как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ако Office вече е инсталиран на RDS сървъра, който използва други абонаменти за Microsoft 365, деинсталирайте го. Например, като отидете на \> контролния панел деинсталиране на програма. Деинсталирайте с помощта [на Поддръжка на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се сближат с проблеми.

4. На RDS сървъра влезте в центъра за администриране на Microsoft 365 с акаунта на администратора и [инсталирайте Приложения на Microsoft 365 за предприятие](https://portal.office.com/OLS/MySoftware.aspx).

5. След инсталирането на ***Office, не отваряйте или не влизайте в*** приложения на Office.

6. На RDS сървъра разрешете активиране на споделен компютър чрез редактиране на системния регистър, като изпълните следните стъпки:

1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете Изпълнение. В полето Отвори въведете **regedit**и след това изберете OK.

2. Изберете Да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени във вашето устройство.

3. В редактора на системния регистър добавете низ стойност на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\СОФТУЕР\Microsoft \Office\ClickToRun\Configuration.

7. На RDS сървъра ***влезте като краен потребител*** и проверете дали активирането на [споделения компютър е разрешено за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

За повече подробности относно предпоставки, инструкции за инсталиране и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [Разполагане на приложения на Microsoft 365 за предприятието чрез услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
За да отстраните грешки, свързани с активирането на споделен компютър, вижте [Отстраняване на проблеми с активирането на споделен компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  