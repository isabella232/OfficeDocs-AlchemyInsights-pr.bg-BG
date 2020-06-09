---
title: Внедряване на екипи като самостоятелни или с нови или съществуващи инсталации на Office
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
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617884"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Внедряване на екипи като самостоятелни или с нови или съществуващи инсталации на Office

Microsoft Teams вече е включен като част от ***новите инсталации*** на приложенията на Microsoft 365 за предприятие, приложения на Microsoft 365 за фирми и Office за Mac. За повече информация вж. [Кога ще започе Microsoft Teams да бъде включен с новите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Освен това, започвайки с версия 1906 в текущия канал , Екипите ще бъдат ***добавени към съществуващите инсталации*** на приложенията на Microsoft 365 за предприятие (и Приложения на Microsoft 365 за бизнеса) на устройства, работещи под Windows, когато актуализирате съществуващата инсталация до най-новата версия. За повече информация вж. [Какво става със съществуващите инсталации на Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Ако не искате да чакате този график за пускане, можете да внедрите Teams като самостоятелен за потребителите си, като [следвате тези инструкции](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)   или можете да накарате потребителите да инсталират Екипи за себе си от  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) .

Ако вашата организация не е готова да разположи екипи, имаме стъпките, които можете да предприемете, за да ***изключите Екипи*** от [нови](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) или [съществуващи](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) инсталации на Office. Ако искате да се инсталирате Teams, но не искате Teams да се стартира автоматично за потребителя, след като е инсталиран, вж. [Предотвратете автоматичното стартиране на Microsoft Teams след инсталиране](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).

За да ***деинсталирайте Teams,*** от устройство, на което се изпълнява Windows, вижте [деинсталиране на Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). За да почистите Екипи на Microsoft от няколко целеви машини или потребители, вижте [Microsoft екипи разполагане почистване](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Ако използвате споделени компютри, услуги за отдалечен работен плот (RDS) или инфраструктура за виртуални работния плот (VDI), вижте [Споделен компютър и VDI среди с Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Ако използвате Office за Mac, вижте [Инсталации на Microsoft Teams на Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> След като Teams е инсталирана, тя [се актуализира автоматично](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) приблизително на всеки две седмици с нови функции и актуализации на качеството. 