---
title: Разполагане Teams като самостоятелни или с нови или съществуващи Office инсталации
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: e8baefafc1c2f9583345779c5ae7a9d3d0e05c4b3b7e1b3a74a9a22f7ceed02a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102191"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Разполагане Teams като самостоятелни или с нови или съществуващи Office инсталации

Microsoft Teams вече е включен като  част от новите инсталации на Приложения на Microsoft 365 за предприятия, Приложения на Microsoft 365 за бизнеса и Office за Mac. За повече информация вж. [Кога ще започе Microsoft Teams да бъде включен с новите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Освен това, започвайки от версия 1906 в текущия  канал, Teams ще бъде добавен към съществуващите инсталации на Приложения на Microsoft 365 за предприятия (и Приложения на Microsoft 365 за бизнеса) на устройства, изпълняващи Windows, когато актуализирате вашата съществуваща инсталация до най-новата версия. За повече информация вж. [Какво става със съществуващите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ако не искате да чакате този график за внедряване, можете да разположите [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) Teams като самостоятелни за вашите потребители, като следвате тези инструкции или можете да закачите вашите потребители да инсталират Teams за себе си [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) от .

Ако вашата организация не е готова да разположи Teams, имаме стъпките, които [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) можете [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) да ***предприемете, за да изключите Teams от*** нови или съществуващи инсталации на Office. Ако искате да се инсталирате Teams, но не искате Teams да се стартира автоматично за потребителя, след като е инсталиран, вж. [Предотвратете автоматичното стартиране на Microsoft Teams след инсталиране](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

За да ***деинсталирайте Teams,*** от устройство, на което се изпълнява Windows, вижте [деинсталиране на Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). За да изчистите Microsoft Teams от няколко целеви машини или потребители, [вж. Microsoft Teams почистване на разполагането](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ако използвате споделени компютри, услуги за отдалечен работен плот (RDS) или инфраструктура за виртуални работния плот (VDI), вижте [Споделен компютър и VDI среди с Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ако използвате Office за Mac, вижте [Инсталации на Microsoft Teams на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> След Teams е инсталиран, той се [актуализира автоматично приблизително на](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) всеки две седмици с нови функции и актуализации на качеството. 