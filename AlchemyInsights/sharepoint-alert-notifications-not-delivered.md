---
title: Известията за известяване на SharePoint не са доставени
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751232"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>Известията за известяване на SharePoint не са доставени

Моля, проверете папката "НЕЖЕЛАНА поща" в имейла си, тъй като понякога предупрежденията могат да отидат там.

Определете дали **не са доставени всички предупреждения** или дали не е доставено **отделно предупреждение** от определен файл или библиотека.

- **Индивидуалните предупреждения не се доставят**: Ако отделно предупреждение от конкретен файл или библиотека не е доставено, можете да се опитате да го изтриете и пресъздадете. Вижте [управление, преглед или изтриване на известия на SharePoint](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) , за да създадете отново известието.
- **Всички предупреждения не се доставят**: Ако всички известявания от множество файлове или библиотеки не се доставят, отидете на [таблото за изправност на услугите](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , за да проверите за всички съвети/събития, които може да възникнат при SharePoint или Exchange. Проблемът може да бъде чрез възможностите за уведомяване на SharePoint или закъсненията в имейли чрез Exchange. Също така ще бъде важно да се отбележи дали се доставя друго имейл съобщение, но ако не е възможно, е вероятно проблемът да е с закъснения на Exchange.

ЧЗВ за известията:

- Не е възможно да се изпращат предупреждения към групата за разпространение, поддържат се само групи за защита и O365.
- Не можете да персонализирате имейл шаблоните за известия; трябва да използвате Microsoft FLOW или SharePoint Designer Workflow, за да ги постигнете.

## <a name="related-topics"></a>Свързани теми

Искате да изпробвате Microsoft Flow в SharePoint online?

- [Създаване на поток](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint и Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
