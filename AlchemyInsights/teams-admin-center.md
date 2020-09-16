---
title: Център за администриране на Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670353"
---
# <a name="teams-admin-center"></a>Център за администриране на Teams

Научете повече за управлението на Teams чрез [Центъра за администриране на Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Ако не можете да получите достъп до Центъра за администриране на Teams, проверете следните неща:

- Уверете се, че сте позволили подходящи [IP адреси за Office 365, както и URL адреса ](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) на всички устройства (защитна стена и т. н.) или в правилата за защитната стена на локалния ви компютър.
- Уверете се, че данните за влизане, които използвате за достъп до портала за администриране на Teams, съвпада с вашето потребителско име, посочено в [портала за администриране на Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).

Ако потребителите не се показват в Центъра за администриране на Teams, проверете следното:

- Създали ли сте потребители или сте дали лицензи през последните 24 часа? Уверете се, че сте изчакали поне 24 часа, преди да отворите билет за поддръжка.
- Уверете се, че сте задали подходящи лицензи?
- Ако имате локален Active Directory, проверете дали [стойността на msRTCSIP-PrimaryUserAddress или SIP адреса в полето ProxyAddresses във вашия локален Active Directory е уникална и форматът съвпада с](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**потребителско име** за потребителя от [центъра за администриране на Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Ако възнамерявате да запазите разгръщане на Skype за бизнеса сървър и да накарате потребителите да се придържат локално и онлайн: Следвайте **"Настройване на хибридно разполагане с Teams и Skype за бизнеса онлайн"** в контролния панел на вашия Skype за бизнеса сървър и преместване на потребители онлайн.
