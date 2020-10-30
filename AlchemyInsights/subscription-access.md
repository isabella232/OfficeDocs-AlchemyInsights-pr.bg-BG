---
title: Достъп за абонамент
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807187"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не можете да влезете в Azure поради проблеми с браузъра (браузърът увисва, запазва завъртането, не се зарежда и т. н.)

Може да ви е повлияна от прекъсване. Проверете дали има текущо прекъсване: [здравен статус на Azure](https://status.azure.com/status/history/).

Моля, излезте от всички активни сесии на Azure. Стартирайте уеб браузър по-личен или инкогнито.

Можете също да се опитате да обновите браузъра, да използвате друг браузър, да изтривате бисквитки от кеша, ако по-горе не работи.

Научете повече: [отстраняване на проблеми при влизане](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Не можете да получите достъп до абонаменти**

В [портала на Azure](https://portal.azure.com/)се уверете, че е избрано правилното Azure Directory от акаунта в горния десен ъгъл.

Уверете се, че в [центъра за акаунти на Azure](https://account.windowsazure.com/Subscriptions)е използван акаунтът.

Научете повече: [отстраняване на неизправности не са намерени абонаменти](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Не можете да получите достъп до хронологията на фактуриране**

Администраторът на акаунта трябва да се увери, че потребителят, който има достъп до информацията за фактуриране, ще бъде добавен в Azure Active Directory като гост потребител: [Добавяне или изтриване на нов потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

След това потребителят трябва да получи роля на глобален администратор: [Присвояване на роля на потребители](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Публикувай това, потребителят може да получи достъп за плащане чрез правилата за RBAC: [предоставяне на достъп до фактурите](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Препоръчвани документи**

-   [Не мога да вляза, за да управлявам абонамента си за Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)