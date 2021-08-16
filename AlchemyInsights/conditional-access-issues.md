---
title: Проблеми с условен достъп
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069953"
---
# <a name="conditional-access-issues"></a>Проблеми с условен достъп

**Отстраняване на проблеми с диагностиката за влизане**

Можете бързо да разберете какво се е случило или да диагностицирате проблеми, свързани с влизането на потребителя, с помощта [на диагностиката за влизане:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Стартирайте диагностиката за влизане.
1. Намерете събитието, за да анализирате, като въведете подробните данни за потребителя, приложението, часа на влизане, ИД на заявка или ИД на корелация.
1. Прегледайте диагностичните резултати, показващи подробностите за случилото се и какви действия можете да предприемете, за да направите промени (ако са необходими някакви промени).

**Стъпки за отстраняване на неизправности при влизане** 

1. Отидете на страницата за влизане в Azure AD.
1. Филтриране на влизания по потребител, времеви диапазон, приложение, състояние, клиентско приложение и т.н.
1. Изберете събитие за влизане и прегледайте раздела Условен достъп, за да видите кои правила са оценени.
1. Щракнете върху реда на правилата, за да видите подробните данни за правилата и да разберете защо е приложен.

**Инструменти за отстраняване на неизправности с правила за условен достъп**

- Режимът само за отчети ви позволява да оценявате правила, без да влияете върху потребителите.
- Инструментът "Какво ако" ви позволява да симулирате събития за влизане и да видите кои правила важат.
- Прозрения и отчетната работна книга показва въздействието в реално време на всяко правило.

**Правила за защита на базова линия**

Правилата за защита на базовата линия са отхвърлени. Те вече не се налагат и скоро ще бъдат премахнати от портала на Azure. Препоръчваме да разрешите настройките [по подразбиране за защита.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

За повече информация относно условен достъп вижте:

[Най-добри практики за условен достъп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Контроли в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Местоположения в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
