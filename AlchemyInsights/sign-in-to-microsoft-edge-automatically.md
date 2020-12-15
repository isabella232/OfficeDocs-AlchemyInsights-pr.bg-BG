---
title: Автоматично влизане в Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676831"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Автоматично влизане в Microsoft Edge

Microsoft Edge използва акаунтът по подразбиране на операционната система, за да записва автоматично потребителя според това как е конфигурирано устройството на потребителя. 

По-долу са описани сценариите за всеки тип конфигурация на устройства и неговия зависим потребителски процес за влизане:

1. **Устройството е хибридно/пад-J**: тази опция е налична в Windows 10, на ниво Windows и съответните версии на сървъра. Потребителите се подписват автоматично със своите акаунти за Azure Active Directory (AD).
2. **Устройството е регистрирано по домейни**: тази опция е налична в Windows 10, на ниво Windows и съответните версии на сървъра. По подразбиране потребителите със акаунти за домейни не се подписват автоматично; за да разрешите автоматичното влизане за тях, използвайте правилата за **ConfigureOnPremisesAccountAutoSignIn** . За да разрешите автоматичното влизане за потребители с акаунти за Azure AD, обмислете хибридно свързване на устройствата.
3. **Акаунтът по подразбиране на операционната система е акаунт в Microsoft**: тази опция е налична в Windows 10 RS3 (версия 1709, компилация 10.0.16299) и по-нови версии. Сценарият е невероятно да се появява на корпоративни устройства. Ако обаче акаунтът по подразбиране на операционната система е акаунт в Microsoft, Microsoft Edge автоматично ще влезе в акаунта на потребителя с акаунт в Microsoft.
 
 
