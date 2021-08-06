---
title: 'RBAC роли '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923115"
---
# <a name="rbac-rules"></a>Правила за RBAC

Ако получите грешката за разрешение: 

- Клиентът с ИД на обект няма разрешение за извършване на действие над обхвата **(код: УдостоверяванеДобра)**: когато се опитате да създадете ресурс, проверете дали в момента сте влезли с потребител, на който е присвоена роля, която има разрешение за запис на ресурса в избрания обхват. Например за да управлявате виртуални машини в група ресурси, трябва да имате ролята "Сътрудник на виртуална [машина"](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в групата ресурси (или родителския обхват). За списък на разрешенията за всяка вградена роля вижте [Вградени роли за ресурси на Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Нямате разрешение да** създавате заявка за поддръжка: когато се опитате да създадете или актуализирате билет за поддръжка, проверете дали в момента сте влезли с потребител, на който е присвоена роля, която има разрешение за Microsoft.Support/supportTickets/write, като например сътрудник на [искане за поддръжка](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- Не могат да се създават повече задачи за роли **(код: RoleAssignmentLimitExceeded)**: когато се опитате да присвоите роля, опитайте да намалите броя на задачите на ролите, като присвоите роли на групи вместо това. Azure поддържа до **2000 задачи** за роли на абонамент.

За повече подробности относно ролите на Azure RBAC вижте [Роли на Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
