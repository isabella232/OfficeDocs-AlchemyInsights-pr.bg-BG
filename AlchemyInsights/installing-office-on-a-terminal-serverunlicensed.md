---
title: Инсталиране на Office на терминален сървър – нелицензиран
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663106"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране на Office на терминален сървър

За разполагане на приложения на Microsoft 365 за Enterprise на сървър с Windows с помощта на услуги за отдалечен работен плот (RDS), наричани преди терминални услуги:
  
- Трябва да имате абонамент за Microsoft 365, включващ приложения на Microsoft 365 за Enterprise, като например Office 365 Enterprise E3 или Enterprise E5. Приложенията Microsoft 365 за бизнеса и приложенията на Microsoft 365 за Business Premium не включват приложенията на Microsoft 365 за Enterprise.

- Трябва да разрешите [активирането на споделен компютър](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ако искате да инсталирате приложенията на Microsoft 365 за Enterprise на RDS от центъра за администриране на Microsoft 365, ***който използва настройките за инсталиране по подразбиране***, използвайте стъпките по-долу.

> [!TIP]
> Можете също да изтеглите и стартирате [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) , за да инсталирате приложенията на Microsoft 365 за Enterprise в режима на активиране на споделен компютър.
  
1. Проверете какво представлява абонаментът за Microsoft 365. [Научете как](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, преминете към друг абонамент за Microsoft 365. [Научете как](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ако Office вече е инсталиран на RDS сървъра с помощта на други абонаменти за Microsoft 365, деинсталирайте го. Например, като отидете в контролния панел, \> Деинсталирайте програма. Деинсталирайте с помощта на [помощника за поддръжка и възстановяване на Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ако се сблъскате с проблеми.

4. На сървъра RDS Влезте в центъра за администриране на Microsoft 365 със своя акаунт на администратор и [Инсталирайте приложенията на Microsoft 365 за Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. След като Office е инсталиран, ***не отваряйте или не влизайте в*** никакви приложения на Office.

6. На RDS Server разрешете активирането на споделен компютър, като редактирате системния регистър, като изпълните следните стъпки:

1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете изпълни. В полето Отвори въведете **regedit**и след това изберете OK.

2. Изберете да, когато бъдете подканени да разрешите на редактора на системния регистър да прави промени на вашето устройство.

3. В редактора на системния регистър Добавете стойност на низ на **SharedComputerLicensing** с настройка 1 под HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. На сървъра RDS ***влезте като краен потребител*** и [се уверете, че активирането на споделен компютър е разрешено за приложенията на Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

За повече информация относно предварителните изисквания, инструкции за настройка и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [разполагане на приложения на Microsoft 365 за Enterprise чрез отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
За да коригирате грешки, свързани с активирането на споделен компютър, вижте [отстраняване на проблеми при активиране на споделен компютър за приложенията Microsoft 365 за Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  