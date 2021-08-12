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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929294"
---
# <a name="create-a-group"></a>Създаване на група

Тази тема описва създаването на групи.

**Разрешение за създаване на група**

Уверете се, че сте упълномощени да създадете нова група. Глобалните администратори могат да забраняват създаването на групи в портала на Azure или панела на Access. Може да се наложи администратор да създаде новата група за вас или да ви даде подходящи разрешения.

**Управление на разрешенията за създаване на група**

1. Глобалните администратори могат да управляват разрешенията за създаване на групи (поради съображения, свързани със защитата) или групите на Office 365, създадени в портала на Azure или панела на Access, като изберат "Потребителите могат да създават групи за защита в порталите на Azure" или "Потребителите могат да създават групи на Office 365 в порталите на Azure" в "Всички групи  >  **общи" (Настройки)**.
2. Можете също да ограничите създаването на група, за да изберете група потребители, ако имате лиценз Azure Active Directory P1 Premium.

**Забраняване на известие за добре дошли за нови Office 365 членове на групата**

Известието за добре дошли, изпратено до потребители, които са добавени към Office 365 групи, може да бъде забранено, като зададете **UnifiedGroupWelcomeMessageEnabled** на False в Powershell. Научете повече за тази настройка [тук](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

