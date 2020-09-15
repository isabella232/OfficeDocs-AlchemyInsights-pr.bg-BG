---
title: Липсващи имейли под карантина
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673703"
---
# <a name="missing-emails-in-quarantine"></a>Липсващи имейли в карантинни "

Администраторите могат да [преглеждат, отделят или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

За да отворите центъра за съответствие на защитата &, отидете на [https://protection.office.com](https://protection.office.com/) . За да отворите страницата карантинни директно, отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Можете да търсите със следните стойности:  

- **ИД на съобщението**: глобален Еднозначен идентификатор на съобщението. Ако изберете съобщение в списъка, в екрана за **подробни данни** на изплаващо, който се появява, се показва СТОЙНОСТТА за **ИД на съобщението** . Администраторите могат да използват [проследяването](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) на съобщенията, за да намират съобщения и СЪОТВЕТНИТЕ им ИД на съобщения.
- **Имейл адрес на подателя**: имейл адресът на един подател.
- **Имейл адрес на получателя**: имейл адресът на един получател.
- **Subject**: използвайте цялата тема на съобщението. Търсенето не различава малки и главни букви.

След като въведете критериите за търсене, щракнете върху обновяване ![ на бутона Обнови, ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** за да филтрирате резултатите.  

Кратките команди, които използвате, за да преглеждате и управлявате съобщения и файлове в карантинни депа, са:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експортиране – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Визуализация – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Имайте предвид, че тази кратка команда е само за съобщения, но не и за зловреден софтуер от ATP за SharePoint Online, OneDrive за бизнеса или Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)