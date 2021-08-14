---
title: Privileged Identity Management роля
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973218"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) роля

**Разрешенията не се предоставят след активирането на роля**

Когато активирате роля в Azure AD Privileged Identity Management (PIM), активирането може да не се разпространи незабавно до всички портали, които изискват привилегированата роля. Понякога дори ако промяната се разпространи, кеширане в уеб в портал може да доведе до това промяната да не влиза в сила веднага.

Ако активирането ви се забави, изпълнете следните стъпки:

1. Излезте от портала на Azure и след това влезте отново. Когато активирате роля на Azure AD или роля на ресурс на Azure, ще видите етапите на активирането. След като всички етапи са завършени, ще видите връзка "Излизане". Можете да използвате тази връзка, за да излезете. Това ще реши повечето случаи за забавяне на активирането.
2. В PIM проверете дали сте в списъка като член на ролята.
3. Ако активирате ролята на администратор на Exchange, се уверете, че сте излезли и влизате отново. Ако проблемът продължава, отворете билет за поддръжка и го повдигнете като проблем. Ако използвате своята роля на Exchange администратор за достъп до центъра за защита и съответствие, вижте следващата стъпка.
4. Ако активирате роля за достъп до центъра за защита и съответствие или ако активирате ролята на администратор на SharePoint, ще изпитате известно забавяне на активирането от няколко минути до няколко часа. Това е известен проблем и ние работим активно с тези екипи, за да разрешим този проблем възможно най-скоро.

За повече информация вижте:

- [Активиране на моите роли на Azure AD в PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Активиране на моите роли на ресурси на Azure в PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Разрешенията не се премахват след дезактивирането на роля или срокът на активиране на роля изтича**

Когато дезактивирате роля в Azure AD Privileged Identity Management когато срокът на активиране на роля изтече, може да има забавяне, където да продължите да имате достъп.

Ако дезактивирането ви се забави, изпълнете следните стъпки:

1. Ако дезактивирате ролята на администратор на Exchange или срокът на активиране на роля изтича и забележите значително забавяне, преди разрешенията да бъдат премахнати, отворете билет за поддръжка и кажете на инженера по поддръжката да ви помогне да подадете билет при екипа за управление на привилегирован достъп (PAM) в Office за този проблем.
2. Ако срокът на активиране е изтекъл, но все още имате отворена сесия на браузъра, затворете браузъра си. Можете да продължите да използвате ролята, докато не затворите тази сесия. Това е известен проблем и ние търсим потенциална корекция, за да анулираме активно всяка сесия, след като активирането е изтекло.

Ако закъснението ви е различно от тези два сценария, отворете билет за поддръжка.
