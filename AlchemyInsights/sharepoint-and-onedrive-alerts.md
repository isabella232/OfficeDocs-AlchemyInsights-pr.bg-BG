---
title: Закъснения при получаване на известия на SharePoint и OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727232"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Закъснения при получаване на известия на SharePoint и OneDrive

- Първо проверете папката Нежелана поща в имейла.
- Ако **всички предупреждения от множество файлове или библиотеки са закъснели**, отидете на [таблото за изправност на услугите](https://portal.office.com/adminportal/home?ref=/servicehealth) , за да проверите за всички съвети/събития, които може да възникнат при SharePoint или Exchange. Възможно е проблемът да е в възможностите за уведомяване на SharePoint или закъсненията в имейли чрез Exchange. Също така имайте предвид, че ако не е получено друго имейл съобщение, проблемът е вероятен при закъснения на Exchange.
- Ако **не е дадено отделно известие от конкретен файл или библиотека**, опитайте да го изтриете и пресъздадете. Вижте [управление, преглед или изтриване на известия на SharePoint](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) , за да създадете отново известието.

> [!NOTE]
> - Известията не могат да бъдат изпратени до група за разпространение. Поддържат се само групи за защита и O365.
> - Не можете да персонализирате шаблоните за имейл известия. Трябва да използвате Microsoft Flow или SharePoint Designer Workflow, за да ги постигнете.
