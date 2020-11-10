---
title: Грешка при влизане в OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982422"
---
# <a name="onedrive-login-error-aadsts50011"></a>Грешка при влизане в OneDrive AADSTS50011

Ако получите съобщение за грешка "AADSTS50011: URL адресът на отговора, зададен в искането, не съответства на отговора" при влизане в приложението OneDrive, проверете за следното:

Вашата версия на OneDrive трябва да е равна или по-голяма от версия 20.052. XXXX. XXXX. За да проверите своята версия, щракнете върху синята икона на OneDrive в областта за уведомяване, изберете **помощ за настройките за & > >**.

Вашата мрежа може да блокира трафика към **g.Live.com** и **oneclient.SFX.MS**. Ако този трафик е блокиран, OneDrive не може да се актуализира. Работете със своя мрежов администратор, за да сте сигурни, че имате достъп до тези URL адреси. [Тези крайни точки](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) трябва да бъдат достъпни за клиенти, използващи планове на Microsoft 365.

Ако трябва ръчно да получите актуална версия на OneDrive, посетете [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
