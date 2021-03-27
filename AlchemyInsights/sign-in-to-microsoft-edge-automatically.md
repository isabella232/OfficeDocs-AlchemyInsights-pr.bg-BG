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
- "8333"
- "9004625"
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398718"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Автоматично влизане в Microsoft Edge

Microsoft Edge използва акаунта по подразбиране за операционната система, за да влиза автоматично в потребител в зависимост от това как е конфигурирано устройството на потребителя. 

Сценариите за конфигурацията на всеки тип устройство и зависимия процес на влизане на потребителите са описани по-долу:

- **Устройството е хибридно/AAD-J:** Тази опция е налична в Windows 10, Windows от ниско ниво и съответните версии на сървъра. Потребителите автоматично са влезли със своите акаунти за Azure Active Directory (AD).
- **Устройството е присъединено към домейн:** Тази опция е налична в Windows 10, Windows от ниско ниво и съответните версии на сървъра. По подразбиране потребителите с акаунти за домейни не са влезли автоматично; за да разрешите автоматичното влизане за тях, използвайте правилата **ConfigureOnPremisesAccountAutoSignIn.** За да разрешите автоматично влизане за потребители с акаунти за Azure AD, помислете за хибридно присъединяване към техните устройства.
- **Акаунтът по** подразбиране на операционната система е акаунт в Microsoft: Тази опция е налична в Windows 10 RS3 (версия 1709, компилация 10.0.16299) и по-нови версии. Сценарият е малко вероятно да възникне на корпоративни устройства. Ако обаче акаунтът по подразбиране за операционната система е акаунт в Microsoft, Microsoft Edge автоматично ще влиза в потребителя с акаунта в Microsoft.
 
 
