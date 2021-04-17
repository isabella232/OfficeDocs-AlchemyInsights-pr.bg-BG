---
title: Създаване на група
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816334"
---
# <a name="create-a-group"></a>Създаване на група

Тази тема описва създаването на групи.

**Разрешение за създаване на група**

Уверете се, че сте упълномощени да създадете нова група. Глобалните администратори могат да забраняват създаването на групи в портала на Azure или панела на Access. Може да се наложи администратор да създаде новата група за вас или да ви даде подходящи разрешения.

**Управление на разрешенията за създаване на група**

1. Глобалните администратори могат да управляват разрешенията за създаване на групи (от съображения, свързани със защитата) или групите на Office 365, създадени в портала на Azure или панела на Access, като изберат "Потребителите могат да създават групи за защита в портали на Azure" или "Потребителите могат да създават групи на Office 365 в порталите на Azure" във всички групи  >  **Общи (Настройки)**.
2. Можете също да ограничите създаването на група, за да изберете група потребители, ако имате лиценз за Azure Active Directory P1 Premium.

**Забраняване на известието за добре дошли за новите членове на групата на Office 365**

Известието за добре дошли, изпратено до потребители, които са добавени към групи на Office 365, може да бъде забранено, като зададете **UnifiedGroupWelcomeMessageEnabled** на False в Powershell. Научете повече за тази настройка [тук](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

