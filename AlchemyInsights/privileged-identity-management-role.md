---
title: Поверителна роля за управление на самоличността
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088516"
---
# <a name="privileged-identity-managementpim-role"></a>Привилегирована роля за управление на самоличността (PIM)

**Не се разрешават разрешения след активирането на роля**

Когато активирате роля в Azure AD поверително управление на самоличността (PIM), активирането може да не се разпространи незабавно във всички портали, които изискват привилегирована роля. Понякога дори ако промяната е размножена, уеб кеширането в портал може да доведе до това, че промяната не влиза в сила незабавно.

Ако активирането ви е отложено, изпълнете следните стъпки:

1. Излезте от портала на Azure и след това влезте отново. Когато активирате РЕКЛАМНА роля на Azure или ресурсна роля на Azure, ще видите етапите на активирането. След като сте завършили всички етапи, ще видите връзката "излизане". Можете да използвате тази връзка, за да излезете. Това ще реши повечето случаи за забавяне на активирането.
2. В PIM Проверете дали сте включени в списъка като член на ролята.
3. Ако активирате ролята на администратор на Exchange, трябва да излезете и да влезете отново. Ако проблемът продължава, отворете билет за поддръжка и го отгледате като проблем. Ако използвате своята роля на администратор на Exchange, за да получите достъп до центъра за сигурност и съответствие, Вижте следващата стъпка.
4. Ако активирате роля за достъп до центъра за защита и съответствие или ако активирате ролята на администратор на SharePoint, ще получите известно закъснение при активирането от няколко минути до няколко часа. Това е известен проблем и активно работим с тези екипи, за да отстраним този проблем възможно най-скоро.

За повече информация вижте:

- [Активиране на моите Azure AD роли в PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Активиране на моите Azure ресурси роли в PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Разрешенията не се премахват, след като дезактивират роля или срокът на активиране на роля изтича**

Когато дезактивирате роля в Azure AD поверително управление на самоличността или когато изтече срокът на активиране на роля, е възможно да има забавяне там, където можете да продължите да имате достъп.

Ако дезактивирането ви е отложено, изпълнете следните стъпки:

1. Ако дезактивирате ролята на администратор на Exchange или срокът на активиране на роля изтича и забелязвате значително забавяне, преди да бъдат премахнати разрешенията, отворете билет за поддръжка и кажете на вашия инженер по поддръжката да ви помогне да подадете билет за този проблем с привилегирования екип за управление на достъпа (PAM).
2. Ако срокът за активиране е изтекъл, но все още имате отворена сесия на браузъра, затворете браузъра си. Можете да продължите да използвате ролята, докато затворите тази сесия. Това е известен проблем и разглеждаме потенциална корекция за активно отменяне на всяка сесия, след като активирането изтече.

Ако закъснението ви е различно от тези два сценария, моля, отворете билет за поддръжка.