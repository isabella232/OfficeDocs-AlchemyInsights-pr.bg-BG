---
title: Разполагане Приложения на Microsoft 365 за предприятия за споделена употреба на RDS, терминален сървър или VDI
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
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325592"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Разполагане Приложения на Microsoft 365 за предприятия за споделена употреба на RDS, терминален сървър или VDI

За да разположите Приложения на Microsoft 365 за предприятия с помощта на услуги за отдалечен работен плот (RDS), наречени преди терминални услуги:

- Трябва да имате план Microsoft 365 за бизнеса или план за Office 365, който включва Приложения на Microsoft 365 за предприятия, като например Office 365 Enterprise E3 или Enterprise E5.
   **Забележка:** Плановете Приложения на Microsoft 365 за бизнеса и Microsoft 365 Business Standard не включват Приложения на Microsoft 365 за предприятия.
- Трябва да разрешите [активирането на споделен компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

**Забележка:** Можете също да изтеглите и изпълните [microsoft Помощник за поддръжка и възстановяване,](https://aka.ms/SaRA_OfficeSCA_M365Portal) за да инсталирате Приложения на Microsoft 365 за предприятия в режим на активиране на споделен компютър.

За повече информация относно предварителните изисквания, инструкциите за настройка и указанията за персонализирани инсталации с помощта на инструмента за разполагане на Office вижте [Разполагане на Приложения на Microsoft 365 за предприятия с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

За да коригирате грешки, свързани с активирането на споделен компютър:

- Вижте [Отстраняване на проблеми с активирането на споделен компютър за Приложения на Microsoft 365 за предприятия](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Вижте [Нулиране на приложенията на Microsoft 365 за състоянието на корпоративно активиране](https://go.microsoft.com/fwlink/?linkid=2109218).

Ако искате да инсталирате Приложения на Microsoft 365 за предприятия на RDS от Център за администриране на Microsoft 365, който използва настройките ***за инсталиране по подразбиране,*** използвайте следните стъпки:

1. Проверете какъв абонамент имате. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ако е необходимо, преминете към друг абонамент. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти на Microsoft, деинсталирайте го. Например, като отивате в **Контролен**  >  **панел Деинсталиране на програма**. Деинсталирайте [с помощта Помощник за поддръжка и възстановяване](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft, ако срещате проблеми.
4. На RDS сървъра влезте в Център за администриране на Microsoft 365 с вашия акаунт на администратор и [инсталирайте Приложения на Microsoft 365 за предприятия.](https://portal.office.com/OLS/MySoftware.aspx)
5. След Office е инсталиран, не отваряйте и ***не влизайте*** в никакви Office приложения.
6. На RDS сървъра разрешете активирането на споделен компютър, като редактирате системния регистър, като изпълните следните стъпки:
   1. Щракнете с десния бутон Windows бутона в долния ляв ъгъл на екрана и изберете **Изпълнение**. В полето Отвори въведете **regedit** и след това изберете **OK**.
   2. Изберете **Да,** когато получите подкана да разрешите на редактора на системния регистър да прави промени във вашето устройство.
   3. В редактора на системния регистър добавете стойност на низ на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. На RDS сървъра влезте като ***краен потребител*** и се уверете, че активирането на споделен [компютър е разрешено за Приложения на Microsoft 365 за предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
