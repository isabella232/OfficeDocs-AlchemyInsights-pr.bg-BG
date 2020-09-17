---
title: Разполагане на Teams като самостоятелно или с нови или съществуващи инсталации на Office
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
ms.openlocfilehash: c3ca4365abc41509ccf602c5b9046655706840fc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806748"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Разполагане на Teams като самостоятелно или с нови или съществуващи инсталации на Office

Microsoft Teams вече е включен като част от ***новите инсталации*** на приложенията на Microsoft 365 за Enterprise, приложенията Microsoft 365 за фирми и Office for Mac. За повече информация вж. [Кога ще започе Microsoft Teams да бъде включен с новите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Освен това, като започнете с версия 1906 в текущия канал, Teams ще бъде ***добавен към съществуващи инсталации*** на приложения на Microsoft 365 за Enterprise (и приложенията на Microsoft 365 за фирми) на устройства, работещи с Windows, когато актуализирате вашата съществуваща инсталация до най-новата версия. За повече информация вж. [Какво става със съществуващите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ако не искате да изчакате този план за внедряване, можете да разположите Teams като самостоятелност за вашите потребители, като [следвате тези инструкции](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   или можете да накарате вашите потребители сами да инсталират екипи  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ако вашата организация не е готова за разполагане на Teams, имаме стъпките, които можете да предприемете, за да ***изключите Teams*** от [нови](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) или [съществуващи](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) инсталации на Office. Ако искате да се инсталирате Teams, но не искате Teams да се стартира автоматично за потребителя, след като е инсталиран, вж. [Предотвратете автоматичното стартиране на Microsoft Teams след инсталиране](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

За да ***деинсталирайте Teams,*** от устройство, на което се изпълнява Windows, вижте [деинсталиране на Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). За да почистите Microsoft Teams от няколко машини за цел или потребители, вижте [разполагане на Microsoft Teams Cleaning](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ако използвате споделени компютри, услуги за отдалечен работен плот (RDS) или инфраструктура за виртуални работния плот (VDI), вижте [Споделен компютър и VDI среди с Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ако използвате Office за Mac, вижте [Инсталации на Microsoft Teams на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> След като Teams е инсталиран, той [автоматично се актуализира](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизително на всеки две седмици с нови функции и актуализации на качеството. 