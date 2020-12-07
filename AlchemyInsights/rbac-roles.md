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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583241"
---
# <a name="rbac-rules"></a>Правила за RBAC

Ако получите съобщение за грешка: 

- **Клиентът с ИД на обекта няма разрешение за извършване на действие по обхват (код: AuthorizationFailed)**: когато се опитате да създадете ресурс, проверете дали сте влезли в момента с потребител, на когото е присвоена роля, която има разрешение за писане на ресурса в избрания обхват. Например, за да управлявате виртуални машини в група ресурси, трябва да имате ролята на [сътрудник за виртуална машина](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) в групата ресурс (или родителен обхват). За списък на разрешенията за всяка вградена роля вижте [вградени роли за ресурси на Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Нямате **разрешение за създаване на заявка за поддръжка**: когато се опитате да създадете или актуализирате билет за поддръжка, проверете дали сте влезли в момента с потребител, на когото е присвоена роля, която има Microsoft. support/supportTickets/write, като например [сътрудник за искане на поддръжка](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Не могат да се създават повече присвоявания на роли (код: RoleAssignmentLimitExceeded)**: когато се опитвате да присвоите роля, опитайте се да намалите броя на присвояванията на роли, като разпределите роля на групи вместо това. Azure поддържа до **2000** присвоявания на роля за абонамент.

За повече информация за ролите в Azure RBAC вижте [ролите в AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
