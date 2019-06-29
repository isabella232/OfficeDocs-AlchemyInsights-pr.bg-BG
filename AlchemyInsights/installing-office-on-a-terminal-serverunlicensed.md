---
title: Инсталиране на office на терминален сървър - нелицензирани
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381718"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране на Office на терминален сървър

За разполагането на Office 365 подпора на Windows Server с помощта на отдалечен работен плот услуги (RDS) по-рано наречена терминални услуги:
  
- Трябва да имате план за Office 365, който включва Office 365 подпора, като Office 365 предприятие E3 или предприятието E5. Office 365 бизнес и Office 365 бизнес Premium планове не включват Office 365 подпора.

- Трябва да разрешите [споделен компютър активиране](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ако искате да инсталирате Office 365 подпора на RDS от портала на Office 365 ** *която използва настройките по подразбиране инсталацията* **, изпълнете следните стъпки:
  
1. Проверете какво Office 365 план имате. [Научете как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, преминаване към различен Office 365 план. [Научете как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ако Office е вече инсталиран на RDS сървъра, използвайки други планове за Office 365, я деинсталирате. Например, като отидете на контролния панел \> деинсталиране на програма. Uninstall using [Microsoft поддръжка и възстановяване помощник](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако работите в изход.

4. На RDS сървъра Влезте в портала на Office 365 с вашия акаунт на администратор и [инсталирате Office 365 подпора](https://portal.office.com/OLS/MySoftware.aspx).

5. След Office е инсталиран, ** *не отвори или да влезете в* ** за приложения на Office.

6. На RDS сървъра разрешите споделен компютър активиране чрез редактиране на системния регистър като следвате тези стъпки:

1. С десния бутон върху бутона на Windows в долния ляв ъгъл на екрана и изберете Run. В полето Отвори въведете **regedit**и след това изберете OK.

2. Отбран да кога суфльор да се даде възможност на редактора на системния регистър да направите промени в устройството.

3. В редактора на системния регистър, добавете низова стойност на **SharedComputerLicensing** с настройка на 1, при HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. На RDS сървъра ** *влизане като краен потребител* ** и се [уверете, че активирането на споделен компютър е разрешен за Office 365 подпора](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

За повече подробности относно предпоставки, настройка на инструкции и насоки за персонализирани инсталации с помощта на инструмента за разполагане на Office вижте [Разполагане на Office 365 подпора с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
За да поправите грешки, свързани с активирането на споделен компютър, моля, вижте [отстраняване на проблеми с активирането на споделен компютър за Office 365 подпора](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  