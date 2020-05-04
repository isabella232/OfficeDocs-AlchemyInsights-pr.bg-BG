---
title: Разполагане на екипи те са самостоятелни или с нови или съществуващи инсталации на Office
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010207"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Разполагане на екипи те са самостоятелни или с нови или съществуващи инсталации на Office

Microsoft Teams вече е включен като част от ***новите инсталации*** на приложенията на Microsoft 365 за предприятие, Microsoft 365 приложения за бизнес а и Office for Mac. За повече информация вж. [Кога ще започе Microsoft Teams да бъде включен с новите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Освен това, започвайки с версия 1906 в месечен канал, Екипи ще бъдат ***добавени към съществуващиинсталации*** на Microsoft 365 приложения за предприятие (и Приложения на Microsoft 365 за бизнеса) на устройства, работещи под Windows, когато актуализирате съществуващата инсталация до най-новата версия. За повече информация вж. [Какво става със съществуващите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ако не искате да чакате този график за пускане, можете да разположите Teams като самостоятелен за вашите потребители, като [следвате тези инструкции](https://docs.microsoft.com/MicrosoftTeams/msi-deployment) или можете да настроите потребителите си да инсталират Teams за себе си. [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

Ако вашата организация не е готова да разположи Teams, ние имаме стъпките, които можете да предприемете, за да ***изключите Екипи*** от [нови](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) или [съществуващи](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) инсталации на Office. Ако искате да се инсталирате Teams, но не искате Teams да се стартира автоматично за потребителя, след като е инсталиран, вж. [Предотвратете автоматичното стартиране на Microsoft Teams след инсталиране](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

За да ***деинсталирайте Teams,*** от устройство, на което се изпълнява Windows, вижте [деинсталиране на Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). За почистване на Microsoft Teams от няколко целеви машини или потребители, вижте [Microsoft Teams разполагане почистване .](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

Ако използвате споделени компютри, услуги за отдалечен работен плот (RDS) или инфраструктура за виртуални работния плот (VDI), вижте [Споделен компютър и VDI среди с Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ако използвате Office за Mac, вижте [Инсталации на Microsoft Teams на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> След инсталирането на Teams автоматично [се актуализира](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) на всеки две седмици с нови функции и актуализации на качеството. 