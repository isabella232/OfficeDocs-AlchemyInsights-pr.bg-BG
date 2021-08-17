---
title: Записване на сайт или списък като шаблон
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109193"
---
# <a name="save-site-or-list-as-a-template"></a>Записване на сайт или списък като шаблон

SharePoint на сайтове са предварително създадени дефиниции, проектирани около определена бизнес нужда. За повече информация вижте Използване [на шаблони за създаване на различни видове SharePoint сайтове](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Ето някои често срещани проблеми/решения относно записването на сайт или списък като шаблон в SharePoint Онлайн.

**Бутонът "Записване на шаблон за сайт/списък" не е наличен или липсва.** 

- Администраторите ще трябва да позволят персонализирания скрипт по избор, за да разрешат функциите на шаблона. За подробни стъпки, примери и съображения вижте Разрешаване или [предотвратяване на скрипт по избор.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Командата "Запиши сайта като шаблон" не се поддържа и може да предизвика проблеми в сайтове, които използват инфраструктурата за публикуване на SharePoint Server.


**Шаблонът за сайт не може да бъде създаден или не работи правилно**

- Възможно е шаблонът да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и да не се активира. Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона за сайт, за да създадете сайт.


- Проверете дали някои списъци или библиотеки [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) надвишават граничния праг за списъчен изглед от 5000 елемента, тъй като това може да блокира създаването на шаблон за сайт.


- Сайтът може да използва твърде много ресурси и следователно шаблонът за сайт надхвърля ограничението от 50 мегабайта (МБ).


- Има проблеми с показването на данни от списък, който използва справочна колона. За повече информация вижте Генериран от шаблон списък не показва данни [от правилния справочен списък в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


За по-подробна информация за често срещани проблеми и решения вижте [Създаване и използване на шаблони за сайтове.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

