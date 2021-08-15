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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026211"
---
# <a name="missing-emails-in-quarantine"></a>Липсващи имейли под карантина"

Администраторите могат [да преглеждат, пускат или изтриват тези съобщения.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

За да отворите центъра за & за съответствие, отидете на [https://protection.office.com](https://protection.office.com/) . За да отворите страницата Карантина директно, отидете на [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Можете да търсите по следните стойности:  

- **ИД на** съобщение: Глобално уникалният идентификатор на съобщението. Ако изберете съобщение в списъка, стойността на  **ИД**  на съобщението се показва в екрана с допълнителни  **данни,**  който се появява. Администраторите могат да използват [проследяване на съобщения,](/microsoft-365/security/office-365-security/message-trace-scc) за да намират съобщения и съответните им стойности за ИД на съобщение.
- **Имейл адрес на подателя:** Имейл адрес на един подател.
- **Имейл адрес на** получателя: Имейл адрес на един получател.
- **Тема:** Използвайте цялата тема на съобщението. Търсенето не е с малки и главни букви.

След като сте въвели критериите за търсене, щракнете върху бутона ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Обнови, за** да филтрирате резултатите.

Кратките команди, които използвате за преглед и управление на съобщения и файлове под карантина, са:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Експортиране-карантинаMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Обърнете внимание, че тази кратка команда е само за съобщения, а не за злонамерени файлове от Microsoft Defender за Office 365 за SharePoint Online, OneDrive за бизнеса или Teams.
- [Съобщение за карантинаMessage](/powershell/module/exchange/release-quarantinemessage)