---
title: Достъп до абонамента
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
ms.openlocfilehash: b138c05e87e70c18bb6528819a34f8a9501446d57dcf4dbac0734f70fbc3466b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999229"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a>Не можете да влезете в Azure поради проблеми с браузъра (браузърът увисва, продължава да се върти, не се зарежда и т.н.)

Възможно е да бъдете засегнати от изтлашване. Проверете дали има продължаващо изтощаване: Състояние на [изтещаване на Azure](https://status.azure.com/status/history/).

Излезте от всички активни сесии на Azure. Стартирайте личен или инкогнито режим на вашия уеб браузър.

Можете също да опитате да обновите браузъра, да използвате друг браузър, да изтриете кеш бисквитките, ако по-горе не работи.

Научете повече: [Отстраняване на проблеми при влизане](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)

**Не може да се получи достъп до абонаменти**

В [портала на Azure](https://portal.azure.com/)се уверете, че правилният указател на Azure е избран от акаунта в горния десен ъгъл.

В центъра [за акаунти в Azure](https://account.windowsazure.com/Subscriptions)се уверете, че използваният акаунт е администраторът на акаунта.

Научете повече: [Отстраняване на неизправности без намерени абонаменти](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)

**Не може да се получи достъп до хронологията на плащанията**

Администраторът на акаунта трябва да се увери, че потребителят, който има достъп до информацията за фактуриране, е добавен в azure Active directory като гост потребител: [Добавяне или изтриване на нов потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

След това на потребителя трябва да бъде дадена роля на глобален администратор: [Дайте роля на потребителите.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)

Публикувайте това, на потребителя може да бъде даден достъп за фактуриране с помощта на правилата на RBAC: [Предоставяне на достъп до фактуриране](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).

**Препоръчителни документи**

-   [Не мога да влизам, за да управлявам абонамента си за Azure](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)