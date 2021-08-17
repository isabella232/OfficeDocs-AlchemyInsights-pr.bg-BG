---
title: Влизане в Microsoft Edge автоматично
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050683"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Влизане в Microsoft Edge автоматично

Microsoft Edge използва акаунта по подразбиране на операционната система, за да влиза автоматично потребител в зависимост от това как е конфигурирано устройството на потребителя. 

Сценариите за конфигурацията на всеки тип устройство и зависимия процес на влизане на потребителите са описани по-долу:

- **Устройството е хибридно/AAD-J:** Тази опция е налична на Windows 10, версията на Windows и съответните версии на сървъра. Потребителите автоматично са влезли със своите Azure Active Directory (AD)акаунти.
- **Устройството е присъединено към домейн:** Тази опция е налична Windows 10 версии на Windows и съответните версии на сървъра. По подразбиране потребителите с акаунти за домейни не са влезли автоматично; за да разрешите автоматичното влизане за тях, използвайте правилата **ConfigureOnPremisesAccountAutoSignIn.** За да разрешите автоматично влизане за потребители с акаунти за Azure AD, помислете за хибридно присъединяване към техните устройства.
- **Акаунтът по** подразбиране на операционната система е акаунт в Microsoft: Тази опция е налична на Windows 10 RS3 (версия 1709, компилация 10.0.16299) и по-нови версии. Сценарият е малко вероятно да възникне на корпоративни устройства. Ако обаче акаунтът по подразбиране на операционната система е акаунт в Microsoft, Microsoft Edge автоматично ще влезете в потребителя с акаунта в Microsoft.
 
 
