---
title: Внедряване на приложения на Microsoft 365 за корпоративни потребители за съвместно използване на RDS, Терминален сървър или VDI
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
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507575"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Внедряване на приложения на Microsoft 365 за корпоративни потребители за съвместно използване на RDS, Терминален сървър или VDI

За да разположите приложения на Microsoft 365 за предприятие, използвайки услуги за отдалечен работен плот (RDS), преди наречени терминални услуги:
- Трябва да имате план на Microsoft 365 за бизнес или план на Office 365, който включва приложения на Microsoft 365 за предприятие, като например Office 365 Enterprise E3 или Enterprise E5.
   > [!NOTE] 
   > Приложенията на Microsoft 365 за бизнеса и плановете на Microsoft 365 Business Premium Standard не включват приложения на Microsoft 365 за предприятие.
- Трябва да разрешите [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Можете също да изтеглите и стартирате помощника за поддръжка на [Microsoft и възстановяване,](https://aka.ms/SaRA_OfficeSCA_M365Portal) за да инсталирате приложения на Microsoft 365 за корпоративни в режим на активиране на споделен компютър.

За повече информация относно предпоставки, инструкции за инсталиране и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте разполагане на [Microsoft 365 приложения за предприятието чрез услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

За да отстраните грешки, свързани с активирането на споделения компютър:
- Вижте [Отстраняване на проблеми с активирането на споделения компютър за приложения на Microsoft 365 за корпоративни](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)клиенти.
- Вижте [Нулиране на приложенията на Microsoft 365 за състоянието на корпоративно активиране](https://go.microsoft.com/fwlink/?linkid=2109218).

Ако искате да инсталирате Приложения на Microsoft 365 за enterprise на RDS от центъра за администриране на Microsoft 365, който използва настройките по подразбиране за ***инсталиране,*** използвайте следните стъпки:

1.    Проверете какъв абонамент имате. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2.    Ако е необходимо, преминете към друг абонамент. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3.    Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти на Microsoft, деинсталирайте го. Например, като отидете в **контролния панел**  >  **Деинсталиране на програма**. Деинсталирайте с помощта [на поддръжката на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако имате проблеми.
4.    На RDS сървъра влезте в центъра за администриране на Microsoft 365 с администраторския си акаунт и [инсталирайте приложения на Microsoft 365 за корпоративни](https://portal.office.com/OLS/MySoftware.aspx).
5.    След инсталирането на Office ***не се отваря или влиза в*** приложения на Office.
6.    RDS сървър разрешаване на активирането на споделения компютър чрез редактиране на системния регистър, като изпълните следните стъпки:
   1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете **Изпълнение**. В полето Отвори въведете **regedit**, след което изберете **OK**.
   2. Изберете **Да,** когато бъдете подканени да разрешите на редактора на системния регистър да прави промени в устройството ви.
   3. В редактора на системния регистър добавете низова стойност **на SharedComputerLicensing** с настройка на 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.
   4. RDS сървър ***влезте като краен потребител*** и проверете дали е разрешено активиране на [споделения компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

