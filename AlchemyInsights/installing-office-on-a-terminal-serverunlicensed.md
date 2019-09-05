---
title: Инсталиране на офис на терминален сървър-неразрешено
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
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735378"
---
# <a name="installing-office-on-a-terminal-server"></a>Инсталиране на Office на терминален сървър

За разполагане на Office 365 ProPlus на Windows Server с помощта на услуги за отдалечен работен плот (RDS), преди наименувани терминални услуги:
  
- Трябва да имате Office 365 план, който включва Office 365 ProPlus, като например Office 365 Enterprise Еi или Enterprise е+. Office 365 бизнес и Office 365 бизнес Премиум планове не включват Office 365 ProPlus.

- Трябва да активирате [споделено активиране на компютъра](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ако искате да инсталирате Office 365 ProPlus на RDS от центъра за администриране на Microsoft 365, ***който използва настройките по подразбиране за инсталиране***, изпълнете следните стъпки:
  
1. Проверете какъв план на Office 365 имате. [Научете как](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ако е необходимо, превключете към друг план на Office 365. [Научете как](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ако Office вече е инсталиран на RDS сървъра, използващ други планове на Office 365, деинсталирайте го. Например, като отидете в контролния панел \> деинсталиране на програма. Деинсталиране с помощта на [Microsoft support и помощник за възстановяване,](https://aka.ms/SARA-OfficeUninstall-Alchemy) ако се занимаваш с проблеми.

4. RDS сървър Влезте в центъра за администриране на Microsoft 365 с администраторски акаунт и [Инсталирайте Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. След инсталирането на Office, ***не отваряйте или влезте в*** приложения на Office.

6. RDS сървър Активирайте активиране на споделен компютър чрез редактиране на системния регистър, като следвате тези стъпки:

1. Щракнете с десния бутон върху бутона Windows в долния ляв ъгъл на екрана и изберете изпълнение. В полето Отвори въведете **regedit**и след това изберете OK.

2. Изберете да, когато бъдете подканени да позволите на редактора на системния регистър да направи промени в устройството.

3. В редактора на системния регистър, добавете низова стойност на **Ssydsлицензиране** с настройка 1 под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \оффице\кликкторун\конфигуратион.

7. RDS сървър, ***влезте като краен потребител*** и [Проверете дали е активирано споделено активиране за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

За повече информация относно предпоставки, настройка на инструкции и указания за персонализирани инсталации с помощта на инструмента за разполагане на Office, вижте [разполагане на office 365 ProPlus с помощта на услуги за отдалечен работен плот](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
За да коригирате грешки, свързани с активирането на споделен компютър, вижте [отстраняване на проблеми при активиране на споделен компютър за Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  