---
title: Инсталиране на office на терминален сървър – нелицензиран
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7e435df1515878ab4fe935ab8148daee29b8e3820095fc6e49db45de4c6279db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055147"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране Office на терминален сървър

За разполагане Приложения на Microsoft 365 за предприятия сървър на Windows с помощта на услуги за отдалечен работен плот (RDS), наречени преди терминални услуги:
  
- Трябва да имате абонамент за Microsoft 365, който включва Приложения на Microsoft 365 за предприятия, като например Office 365 Enterprise E3 или Enterprise E5. Плановете Приложения на Microsoft 365 за бизнеса и Приложения на Microsoft 365 за бизнеса Premium не включват Приложения на Microsoft 365 за предприятия.

- Трябва да разрешите [активирането на споделен компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ако искате да инсталирате Приложения на Microsoft 365 за предприятия на RDS от Център за администриране на Microsoft 365, който използва настройките ***за инсталиране по подразбиране,*** използвайте следните стъпки.

> [!TIP]
> Можете също да изтеглите и стартирате [microsoft Помощник за поддръжка и възстановяване,](https://aka.ms/SaRA_OfficeSCA_M365Portal) за да Приложения на Microsoft 365 за предприятия в режим на активиране на споделен компютър.
  
1. Проверете Microsoft 365 абонамента, който имате. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, преминете към друг Microsoft 365 абонамент. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ако Office вече е инсталиран на RDS сървъра с помощта на други Microsoft 365 абонаменти, деинсталирайте го. Например, като отивате в Контролен \> панел Деинсталиране на програма. Деинсталирайте [с помощта Помощник за поддръжка и възстановяване](https://aka.ms/SARA-OfficeUninstall-Alchemy) Microsoft, ако срещате проблеми.

4. На RDS сървъра влезте в Център за администриране на Microsoft 365 вашия акаунт на администратор и [инсталирайте Приложения на Microsoft 365 за предприятия.](https://portal.office.com/OLS/MySoftware.aspx)

5. След Office е инсталиран, ***не отваряйте и не влизайте*** в никакви Office приложения.

6. На RDS сървъра разрешете активирането на споделен компютър, като редактирате системния регистър, като изпълните следните стъпки:

1. Щракнете с десния бутон Windows бутона в долния ляв ъгъл на екрана и изберете Изпълнение. В полето Отвори въведете **regedit** и след това изберете OK.

2. Изберете Да, когато получите подкана да разрешите на редактора на системния регистър да прави промени във вашето устройство.

3. В редактора на системния регистър добавете стойност на низ на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На RDS сървъра влезте като ***краен потребител*** и се уверете, че активирането на [споделен компютър е разрешено за Приложения на Microsoft 365 за предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

За повече подробности относно предварителните изисквания, инструкциите за настройка и указанията за персонализирани инсталации с помощта на инструмента за разполагане на Office вижте [Разполагане на Приложения на Microsoft 365 за предприятия с помощта на услугите за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
За да коригирате грешки, свързани с активирането на споделен компютър, вижте Отстраняване на проблеми с [активирането на споделен компютър за Приложения на Microsoft 365 за предприятия.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)
  