---
title: Липсващи имейли под карантина
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831723"
---
# <a name="missing-emails-in-quarantine"></a>Липсващи имейли под карантина"

Администраторите могат [да преглеждат, пускат или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

За да отворите центъра за & за съответствие, отидете на [https://protection.office.com](https://protection.office.com/) . За да отворите страницата Карантина директно, отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Можете да търсите по следните стойности:  

- **ИД на** съобщение: Глобално уникалният идентификатор на съобщението. Ако изберете съобщение в списъка, стойността на  **ИД**  на съобщението се показва в екрана с допълнителни  **данни,**  който се появява. Администраторите могат да използват [проследяване на съобщения,](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) за да намират съобщения и съответните им стойности за ИД на съобщение.
- **Имейл адрес на подателя:** Имейл адрес на един подател.
- **Имейл адрес на** получателя: Имейл адрес на един получател.
- **Тема:** Използвайте цялата тема на съобщението. Търсенето не е с малки и главни букви.

След като сте въвели критериите за търсене, щракнете върху бутона ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обнови, за** да филтрирате резултатите.  

Кратките команди, които използвате за преглед и управление на съобщения и файлове под карантина, са:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експортиране-карантинаMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обърнете внимание, че тази кратка команда е само за съобщения, а не за злонамерени файлове от ATP за SharePoint Online, OneDrive за бизнеса или Teams.
- [Съобщение за карантинаMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)