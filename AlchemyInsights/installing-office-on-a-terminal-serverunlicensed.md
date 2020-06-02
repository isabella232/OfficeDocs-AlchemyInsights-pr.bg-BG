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
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508617"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране на Office на терминален сървър

За разполагане на приложения на Microsoft 365 за enterprise на сървър на Windows с помощта на услуги за отдалечен работен плот (RDS), по-рано наречени терминални услуги:
  
- Трябва да имате абонамент за Microsoft 365, който включва приложения на Microsoft 365 за корпоративни организации, като например Office 365 Enterprise E3 или Enterprise E5. Приложенията на Microsoft 365 за бизнеса и приложенията на Microsoft 365 за бизнес премиум планове не включват приложения на Microsoft 365 за предприятие.

- Трябва да активирате [активирането на споделения компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ако искате да инсталирате Приложения на Microsoft 365 за enterprise на RDS от центъра за администриране на Microsoft 365, който използва настройките по подразбиране за ***инсталиране,*** използвайте следните стъпки.

> [!TIP]
> Можете също да изтеглите и стартирате помощника за поддръжка на [Microsoft и възстановяване,](https://aka.ms/SaRA_OfficeSCA_M365Portal) за да инсталирате приложения на Microsoft 365 за корпоративни в режим на активиране на споделен компютър.
  
1. Проверете какво имате абонамент за Microsoft 365. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, преминете към друг абонамент за Microsoft 365. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти на Microsoft 365, деинсталирайте го. Например, като отидете в контролния панел \> Деинсталиране на програма. Деинсталирайте с помощта [на поддръжката на Microsoft и помощника за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако имате проблеми.

4. На RDS сървъра влезте в центъра за администриране на Microsoft 365 с администраторския си акаунт и [инсталирайте приложения на Microsoft 365 за корпоративни](https://portal.office.com/OLS/MySoftware.aspx).

5. След инсталирането на Office ***не се отваря или влиза в*** приложения на Office.

6. RDS сървър разрешаване на активирането на споделения компютър чрез редактиране на системния регистър, като изпълните следните стъпки:

1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете Изпълнение. В полето Отвори въведете **regedit**и след това изберете OK.

2. Изберете Да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени в устройството ви.

3. В редактора на системния регистър добавете низова стойност **на SharedComputerLicensing** с настройка на 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\ClickToRun\Configuration.

7. RDS сървър ***влезте като краен потребител*** и проверете дали е разрешено активиране на [споделения компютър за Приложения на Microsoft 365 за предприятие](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

За повече информация относно предпоставките, инструкциите за инсталиране и указанията за потребителски инсталации с помощта на инструмента за разполагане на Office вижте разполагане на [Приложения на Microsoft 365 за предприятието с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
За да отстраните грешки, свързани с активирането на споделения компютър, вижте [Отстраняване на проблеми със споделените активиране на компютъра за Приложения на Microsoft 365 за корпоративни](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  