---
title: Свързване към модула MSCommerce
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
- "9001212"
- "3529"
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974658"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce изисква акаунт на администратор на фирма или фактуриране

Модулът MSCommerce изисква акаунт с привилегии на администратор на фирма или фактуриране. Ако получавате следната грешка, ще трябва да се свържете отново с друг акаунт.

*ErrorMessage – Отдалеченият сървър върна грешка: (403) Забранено. ГрешкаДетайли – при C:\Програмни файлове\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Неуспешно претриване ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Грешка при запис], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Напълно квалифициранErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ако вашият акаунт няма привилегии на администратор на фирма или фактуриране, се обърнете към своя ИТ администратор.
