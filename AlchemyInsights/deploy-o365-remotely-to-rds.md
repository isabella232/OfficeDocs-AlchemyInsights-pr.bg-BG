---
title: Разполагане на Приложения на Microsoft 365 за корпоративно за споделено използване на RDS, терминален сървър или VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704694"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Разполагане на Приложения на Microsoft 365 за корпоративно за споделено използване на RDS, терминален сървър или VDI

За разполагане на Приложения на Microsoft 365 за предприятие с помощта на услугите за отдалечен работен плот (RDS), наричани преди терминални услуги:
- Трябва да имате план на Microsoft 365 за бизнеса или план на Office 365, който включва приложения на Microsoft 365 за предприятие, като например Office 365 Enterprise E3 или Enterprise E5.
   > [!NOTE] 
   > Плановете на Microsoft 365 за бизнеса и стандартните бизнес планове на Microsoft 365 не включват приложенията на Microsoft 365 за предприятие.
- Трябва да разрешите [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Можете също да изтеглите и стартирате поддръжката на [Microsoft и помощника](https://aka.ms/SaRA_OfficeSCA_M365Portal) за възстановяване, за да инсталирате Приложения на Microsoft 365 за предприятие в режим на активиране на споделен компютър.

За повече информация относно предпоставки, инструкции за инсталиране и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [Разполагане на приложения на Microsoft 365 за предприятието с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

За да отстраните грешки, свързани с активирането на споделен компютър:
- Вижте [отстраняване на проблеми при активиране на споделен компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Вижте [Нулиране на приложенията на Microsoft 365 за състоянието на корпоративно активиране](https://go.microsoft.com/fwlink/?linkid=2109218).

Ако искате да инсталирате Microsoft 365 приложения за предприятие на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране,*** използвайте следните стъпки:

1.    Проверете какъв абонамент имате. [Научете как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    Ако е необходимо, преминете към друг абонамент. [Научете как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    Ако Office вече е инсталиран на RDS сървъра, който използва други абонаменти на Microsoft, деинсталирайте го. Например, като отидете **на Контролния панел** > **Деинсталиране на програма**. Деинсталирайте с помощта [на Поддръжка на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се сближат с проблеми.
4.    На RDS сървъра влезте в центъра за администриране на Microsoft 365 с акаунта на администратора и [инсталирайте Приложения на Microsoft 365 за предприятие](https://portal.office.com/OLS/MySoftware.aspx).
5.    След инсталирането на ***Office, не отваряйте или не влизайте в*** приложения на Office.
6.    На RDS сървъра разрешете активиране на споделен компютър чрез редактиране на системния регистър, като изпълните следните стъпки:
   1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете **Изпълнение**. В полето Отвори въведете **regedit**и след това изберете **OK**.
   2. Изберете **Да,** когато бъдете подканени да разрешите на редактора на системния регистър да прави промени във вашето устройство.
   3. В редактора на системния регистър добавете низ стойност на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\СОФТУЕР\Microsoft \Office\ClickToRun\Configuration.
   4. На RDS сървъра ***влезте като краен потребител*** и проверете дали активирането на [споделения компютър е разрешено за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

