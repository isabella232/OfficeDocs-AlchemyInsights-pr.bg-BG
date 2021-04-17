---
title: Свързване към модула на MSCommerce
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
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829725"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce изисква акаунт на администратор на фирма или фактуриране

Модулът MSCommerce изисква акаунт с привилегии на администратор на фирма или фактуриране. Ако получавате следната грешка, ще трябва да се свържете отново с друг акаунт.

*ErrorMessage – Отдалеченият сървър върна грешка: (403) Забранено. ГрешкаДетайли – при C:\Програмни файлове\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Неуспешно претриване ...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo : NotSpecified: (:) [Грешка при запис], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ Напълно квалифициранErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ако вашият акаунт няма привилегии на администратор на фирма или фактуриране, се обърнете към своя ИТ администратор.
