---
title: Отчетите в Център за администриране на Microsoft 365 не показват четими потребителско име
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2021
ms.locfileid: "59315822"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Отчетите в Център за администриране на Microsoft 365 не показват четими потребителско име

Отчетите в Център за администриране на Microsoft 365 не показват потребителски имена, а вместо това показват алфа-числови стойности, като например B2BC6C15BB9FCDEA71E5CD302D228CC8.

Това е очаквано поведение и е съобщено в центъра за съобщения (MC275344, публикувано на 3 август 2021 г.). 

Глобалните администратори могат да връщат тази промяна за своя клиент и да показват разпознаваема потребителска информация, ако техните практики за поверителност на организацията позволяват това. За да върнете промяната за клиента:

1. В центъра за администриране отидете **на Настройки**  >  **на org**  >  [**Services**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services)и изберете **Отчети**. 
1. Под **Изберете как да покажете информацията за потребителя** изберете Показване на **идентифицираща потребителска информация в** отчетите и след това стартирайте отново отчета.