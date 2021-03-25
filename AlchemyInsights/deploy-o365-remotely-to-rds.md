---
title: Разполагане на приложения на Microsoft 365 за Enterprise за споделена употреба на RDS, терминалния сървър или VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200662"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Разполагане на приложения на Microsoft 365 за Enterprise за споделена употреба на RDS, терминалния сървър или VDI

За да разположите приложенията на Microsoft 365 за Enterprise чрез Remote Desktop Services (RDS), наричани преди терминални услуги:

- Трябва да имате план на Microsoft 365 за фирми или план на Office 365, който включва приложенията на Microsoft 365 за Enterprise, като например Office 365 Enterprise E3 или Enterprise E5.
   > [!NOTE]
   > Приложенията Microsoft 365 за бизнеса и Microsoft 365 Business Standard не включват приложенията на Microsoft 365 за Enterprise.
- Трябва да разрешите [активирането на споделен компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Можете също да изтеглите и стартирате [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , за да инсталирате приложенията на Microsoft 365 за Enterprise в режима на активиране на споделен компютър.

За повече информация относно предварителни изисквания, инструкции за настройка и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office вижте [разполагане на приложения на Microsoft 365 за Enterprise чрез отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

За да коригирате грешки, свързани с активирането на споделен компютър:

- Вижте [отстраняване на проблеми при активиране на споделен компютър за приложенията Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Вижте [Нулиране на приложенията на Microsoft 365 за състоянието на корпоративно активиране](https://go.microsoft.com/fwlink/?linkid=2109218).

Ако искате да инсталирате приложенията на Microsoft 365 за Enterprise на RDS от центъра за администриране на Microsoft 365, ***който използва настройките за инсталиране по подразбиране***, използвайте следните стъпки:

1. Проверете какви абонаменти имате. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ако е необходимо, преминете към друг абонамент. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти за Microsoft, деинсталирайте го. Например, като отидете в **контролния панел**,  >  **Деинсталирайте програма**. Деинсталирайте с помощта на [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ако се сблъскате с проблеми.
4. На сървъра RDS Влезте в центъра за администриране на Microsoft 365 със своя акаунт на администратор и [Инсталирайте приложенията на Microsoft 365 за Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. След като Office е инсталиран, ***не отваряйте или не влизайте в*** никакви приложения на Office.
6. На RDS Server разрешете активирането на споделен компютър, като редактирате системния регистър, като изпълните следните стъпки:
   1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете **изпълнение**. В полето Отвори въведете **regedit** и след това изберете **OK**.
   2. Изберете **да** , когато бъдете подканени да разрешите на редактора на системния регистър да прави промени на вашето устройство.
   3. В редактора на системния регистър Добавете стойност на низ на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На сървъра RDS ***влезте като краен потребител*** и [се уверете, че активирането на споделен компютър е разрешено за приложенията на Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
