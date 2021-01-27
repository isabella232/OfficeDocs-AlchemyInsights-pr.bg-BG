---
title: Проблеми с достъпа под условие
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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014722"
---
# <a name="conditional-access-issues"></a>Проблеми с достъпа под условие

**Отстраняване на проблеми с диагностичната идентификация**

Можете бързо да разберете какво се е случило или да диагностицирате проблеми, свързани с потребителското влизане, като използвате [диагностичната диагностика за влизане](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Стартирайте диагностичната диагностика за влизане.
1. Намерете събитието, което искате да анализирате, като въведете подробностите, които имате за потребителя, приложението, часа на влизане, ИД на заявката или ИД на корелация.
1. Прегледайте диагностичните резултати, показващи подробностите за това какво се е случило и какви действия можете да предприемете, за да направите промени (ако са необходими промени).

**Стъпки за отстраняване на неизправности при влизане** 

1. Придвижете се до страницата за влизане на Azure AD.
1. Филтрирайте регистрациите по потребител, времеви диапазон, приложение, състояние, клиентско приложение и т. н.
1. Изберете събитие за влизане и Прегледайте раздела условен достъп, за да видите кои правила са оценени.
1. Щракнете върху реда на правилата, за да видите подробните данни за правилата и да разберете защо то е приложено.

**Инструменти за отстраняване на неизправности при правила за условен достъп**

- Режим само за отчети ви позволява да оценявате правила, без да засягате потребители.
- Инструментът If ви позволява да симулирате събития при влизане и да виждате кои правила се прилагат.
- Работна книга за прозрения и отчитане показва въздействието в реално време на всяка политика.

**Правила за защита на базова линия**

Правилата за защита на базисни стойности бяха прекратени. Те вече не се налагат и скоро ще бъдат премахнати от портала на Azure. Препоръчваме ви да разрешавате [настройките по подразбиране за защита](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

За повече информация относно условния достъп вижте:

[Най-добри практики за условен достъп в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Условия в условния достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Контроли в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Местоположения в условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
