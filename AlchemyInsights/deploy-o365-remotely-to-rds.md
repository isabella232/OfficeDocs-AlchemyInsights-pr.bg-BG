---
title: Разполагане на Office 365 ProPlus за споделено използване на RDS, терминален сървър или VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959449"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Разполагане на Office 365 ProPlus за споделено използване на RDS, терминален сървър или VDI

За разполагане на Office 365 ProPlus с помощта на услуги за отдалечен работен плот (RDS), преди наименувани терминални услуги:
- Трябва да имате Microsoft 365 за бизнес план или Office 365 план, който включва Office 365 ProPlus, като например Office 365 Enterprise Еi или Enterprise е+.
   > [!NOTE] 
   > Office 365 бизнес и Office 365 бизнес Премиум планове не включват Office 365 ProPlus.
- Трябва да активирате [споделено активиране на компютъра](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Можете също да изтеглите и стартирате [Microsoft поддръжка и възстановяване помощник](https://aka.ms/SaRA_OfficeSCA_M365Portal) за инсталиране на Office 365 ProPlus в режим на споделена компютърна активация.

За повече информация относно предпоставки, инструкции за инсталиране и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office вижте [разполагане на office 365 ProPlus с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

За да коригирате грешки, свързани с активирането на споделен компютър:
- Вижте [отстраняване на проблеми с активиране на споделен компютър за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Вижте [нулиране Office 365 ProPlus активиране състояние](https://go.microsoft.com/fwlink/?linkid=2109218).

Ако искате да инсталирате Office 365 ProPlus на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране***, използвайте следните стъпки:

1.  Проверете какъв план на Office 365 имате. [Научете как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  Ако е необходимо, превключете към друг план на Office 365. [Научете как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  Ако Office вече е инсталиран на RDS сървъра, използващ други планове на Office 365, деинсталирайте го. Например, като отидете на **контролния панел** > **Деинсталиране на програма**. Деинсталиране с помощта на [Microsoft support и помощник за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се занимаваш с проблеми.
4.  RDS сървър Влезте в центъра за администриране на Microsoft 365 с администраторски акаунт и [Инсталирайте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  След инсталирането на Office, ***не отваряйте или влезте в*** приложения на Office.
6.  RDS сървър Активирайте активиране на споделен компютър чрез редактиране на системния регистър, като следвате тези стъпки:
   1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете **Run**. В полето Отвори въведете **regedit**и след това изберете **OK**.
   2. Изберете " **да** ", когато получите подкана да позволите на редактора на системния регистър да прави промени в устройството.
   3. В редактора на системния регистър, добавете низ стойност на **Sedimлицензиране** с настройка 1 под HKEY_LOCAL_MACHINE \ софтуер \ Microsoft \оффице\кликкторун\конфигуратион.
   4. RDS сървър, ***влезте като краен потребител*** и [Проверете дали е активирано споделено активиране за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

