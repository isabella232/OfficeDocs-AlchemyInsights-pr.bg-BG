---
title: Разполагане Приложения на Microsoft 365 за споделена употреба на RDS, терминален сървър или VDI
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077239"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>Разполагане Приложения на Microsoft 365 за споделена употреба на RDS, терминален сървър или VDI

За да разположите Приложения на Microsoft 365 с помощта на услуги за отдалечен работен плот (RDS), бивши терминални услуги, трябва:

- Използвайте лесната корекция, за да разрешите TLS 1.2 по подразбиране, ако използвате по-стара версия на Windows (например Windows 7 SP1, Windows Server 2008 R2). За лесна корекция и повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)като защитени протоколи по подразбиране в WinHTTP в Windows. 
- Имате план, който включва Приложения на Microsoft 365 за предприятия (преди Office 365 Plus). Например Office 365 E3 или Microsoft 365 E5 или всеки план, който включва настолната версия на Project или Visio, като например Project (план 3) или Visio (план 2), или плана Microsoft 365 Business Premium, който включва и Приложения на Microsoft 365 за бизнеса.
- Разрешаване на активирането на споделен компютър. За повече информация вижте Общ [преглед на активирането на споделен компютър за Приложения на Microsoft 365](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**Забележка:** За да Приложения на Microsoft 365 в режим на активиране на споделен компютър, изтеглете и стартирайте [microsoft Помощник за поддръжка и възстановяване](https://aka.ms/SaRA_OfficeSCA_M365Portal). За подробности относно предварителните изисквания, инструкциите за настройка и указанията за персонализиране на инсталациите с помощта на инструмента за разполагане на Office вижте [Разполагане на Приложения на Microsoft 365 с](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)помощта на услуги за отдалечен работен плот .

За да коригирате грешки, свързани с активирането на споделен компютър, вижте:

- [Отстраняване на проблеми с активирането на споделен компютър за Приложения на Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Нулиране на Приложения на Microsoft 365 за предприятия на активиране](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ако искате да инсталирате Приложения на Microsoft 365 на RDS от Център за администриране на Microsoft 365, който използва настройките за инсталиране по подразбиране, изпълнете следните стъпки:

1. Проверете какъв Microsoft 365 имате. За повече информация вижте [Какъв абонамент имам?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Ако е необходимо, преминете към друг Microsoft 365 план. За повече информация вижте [Надстройване до друг план](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Ако Приложения на Microsoft 365 вече е инсталиран на RDS сървъра с помощта на други несъвместими планове, деинсталирайте го, като изберете **Деинсталиране на** програма от  >  **контролния панел.** Ако имате проблеми, деинсталирайте, като изтеглите [Microsoft Помощник за поддръжка и възстановяване](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. На RDS сървъра влезте в Център за администриране на Microsoft 365 вашия акаунт на администратор и [инсталирайте Office.](https://portal.office.com/OLS/MySoftware.aspx)

   След Office е инсталиран, не отваряйте и не влизайте в никакви Office приложения.

1. На RDS сървъра разрешете активирането на споделен компютър, като редактирате системния регистър:

   1. Щракнете с десния бутон Windows бутона в долния ляв ъгъл на екрана и изберете **Изпълнение**. В полето Отвори въведете **regedit** и след това изберете **OK**.

   1. Когато получите подкана да разрешите на редактора на системния регистър да прави промени на вашето устройство, изберете **Да**.

   1. В редактора на системния регистър, под HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration добавете стойност на низ на **SharedComputerLicensing** с настройка **1** .

1. На RDS сървъра влезте като краен потребител и се уверете, че активирането на споделен компютър е разрешено за Приложения на Microsoft 365. 

   За подробности вижте Проверка [дали активирането на споделен компютър е разрешено за Приложения на Microsoft 365](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).