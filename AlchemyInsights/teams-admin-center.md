---
title: Център за администриране на Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 29e54e0f8255b4ce84c433f2cc827aaedf35327626f0095788faef802763bc53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049333"
---
# <a name="teams-admin-center"></a>Център за администриране на Teams

Научете повече за управлението на Teams чрез [Центъра за администриране на Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ако не можете да получите достъп до Центъра за администриране на Teams, проверете следните неща:

- Уверете се, че сте позволили подходящи [IP адреси за Office 365, както и URL адреса ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всички устройства (защитна стена и т. н.) или в правилата за защитната стена на локалния ви компютър.
- Уверете се, че данните за влизане, които използвате за достъп до портала за администриране на Teams, съвпада с вашето потребителско име, посочено в [портала за администриране на Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ако потребителите не се показват в Центъра за администриране на Teams, проверете следното:

- Създали ли сте потребители или сте дали лицензи през последните 24 часа? Уверете се, че сте изчакали поне 24 часа, преди да отворите билет за поддръжка.
- Уверете се, че сте задали подходящи лицензи?
- Ако имате локален Active Directory, проверете дали стойността [на msRTCSIP-PrimaryUserAddress](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) или SIP адреса в полето ProxyAddresses във вашия локален Active Directory е уникална и форматът съответства на глътка:**Потребителско** име на потребителя [от Център за администриране на Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ако възнамерявате да поддържате разполагане на Skype за бизнеса сървър и потребителите да се разполагат локално и онлайн: следвайте "Настройване на хибридно **разполагане с Teams и Skype за бизнеса Online"** във вашия контролен панел на Skype за бизнеса сървър и преместване на потребители онлайн.
