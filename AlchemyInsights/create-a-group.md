---
title: Създаване на група
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088519"
---
# <a name="create-a-group"></a>Създаване на група

Тази тема описва създаването на групи.

**Разрешение за създаване на група**

Уверете се, че сте упълномощени да създавате нова група. Глобалните администратори могат да забранят създаването на групи в портала на Azure или панела на Access. Може да ви е нужен администратор, за да създадете новата група вместо вас или за да ви бъдат дадени подходящи разрешения.

**Управление на разрешения за създаване на група**

1. Глобалните администратори могат да управляват разрешенията за създаване на групи (за свързани със защитата причини) или групи на Office 365, създадени в портала на Azure или **панела на Access**, като изберете "потребители могат да създадат групи за защита в Azure Portals" или "потребителите могат да създават групи на Office 365 в Azure Portals"  >  **General (Settings)**
2. Можете също да ограничите създаването на групи, за да изберете група от потребители, ако имате лиценз за Azure Active Directory P1 Premium.

**Забраняване на добре дошли уведомявания за нови членове на групата на Office 365**

Известието за добре дошли, изпратено до потребители, които са добавени към групите на Office 365, могат да бъдат забранени чрез задаване на **UnifiedGroupWelcomeMessageEnabled** на FALSE в PowerShell. Запознайте се с тази настройка [тук](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

