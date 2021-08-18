---
title: OneDrive за влизане AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112901"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive за влизане AADSTS50011

Ако получите грешка "AADSTS50011: URL адресът на отговора, зададен в искането, не отговаря на отговора", когато влезете в приложението OneDrive, проверете за следното:

Вашата OneDrive версия трябва да е равна или по-голяма от версия 20.052.XXXX.XXXX. За да проверите вашата версия, щракнете върху синята OneDrive в областта за уведомяване, изберете **Помощ & Настройки > Настройки > За**.

Вашата мрежа може да блокира трафика **g.live.com и** **oneclient.sfx.ms**. Ако този трафик е блокиран, OneDrive не може да се актуализира. Работете с вашия мрежов администратор, за да се уверите, че имате достъп до тези URL адреси. [Тези крайни точки трябва](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) да са достъпни за клиенти, които използват Microsoft 365 планове.

Ако трябва ръчно да получите текуща версия на OneDrive, посетете [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
