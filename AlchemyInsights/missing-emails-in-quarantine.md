---
title: Липсващи имейли в карантина
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/03/2020
ms.locfileid: "44568920"
---
# <a name="missing-emails-in-quarantine"></a>Липсващи имейли в карантина"

Администраторите могат да [преглеждат, освобождават или изтриват тези съобщения.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

За да отворите Центъра за съответствие на & за защита, отидете на [https://protection.office.com](https://protection.office.com/) . За да отворите директно страницата "Карантина", отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Можете да търсите по следните стойности:  

- **ИД**на съобщение : Глобално еднозначен идентификатор на съобщението. Ако изберете съобщение в списъка, стойността на **ИД** на съобщение се появява в екрана за допълнителни **подробности,** който се появява. Администраторите могат да използват [съобщение за проследяване](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) за намиране на съобщения и съответните им стойности за ИД на съобщение.
- **Имейл адрес на подателя:** Имейл адрес на един единствен подател.
- **Имейл адрес на получателя:** Имейл адрес на един получател.
- **Относно:** Използвайте целия предмет на съобщението. Търсенето не е от значение за малките и главните букви.

След като въведете критериите за търсене, щракнете върху ![ Бутона ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обновяване,** за да филтрирате резултатите.  

Кратките команди, които използвате за преглед и управлява съобщения и файлове в карантина са:
- [Изтриване на карантинаСъсижен](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експортиране-карантинаСъсище](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Получаване на карантина:](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Визуализация-карантинаСъс кутия:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Имайте предвид, че тази команда е само за съобщения, а не зловреден софтуер файлове от ATP за SharePoint Online, OneDrive за бизнес или екипи.
- [Карантина за освобождаване](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)