---
title: Отчетите в Център за администриране на Microsoft 365 не показват четимо потребителско име
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
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327803"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Отчетите в Център за администриране на Microsoft 365 не показват четимо потребителско име

Отчетите в центъра за администриране на Microsoft 365 не показват потребителски имена, а показват буквено-цифрови стойности, като например B2BC6C15BB9FCDEA71E5CD302D228CC8.

Това е очаквано поведение и е съобщено в центъра за съобщения (MC275344, публикувано на 3 август 2021 г.). 

Глобалните администратори могат да върнат тази промяна за своя клиент и да покажат информация за потребителя, която може да бъде идентифицирана, ако практиките за поверителност на организацията им позволяват. За да върнете промяната за клиента:

1. В центъра за администриране отидете **Настройки** > **Настройки на организацията** > [**Услуги**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services )и изберете **Отчети**. 
1. Под **Изберете как да се показва информацията за потребителя** изберете **Показване на информация за идентифициращия потребител в отчетите** и след това изпълнете отново отчета.