---
title: Създаване на сайт в SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052458"
---
# <a name="create-sharepoint-sites-using-templates"></a>Създаване на сайтове на SharePoint с помощта на шаблони

Шаблоните за сайтове на SharePoint са предварително построени дефиниции, проектирани около конкретна бизнес потребност. За повече информация вижте [използване на шаблони за създаване на различни видове сайтове на SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Ето някои често срещани проблеми/решения по отношение на записването на сайт или списък като шаблон в SharePoint online. 

**Бутонът за запис на шаблон за сайт/списък не е наличен или липсва**

Администраторите ще трябва да разрешат персонализирания скрипт, за да разрешат функциите на шаблона. За подробни стъпки, примери и съображения вижте 

- [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Командата за записване на сайта като шаблон не се поддържа и може да доведе до проблеми на сайтове, използващи инфраструктура за публикуване на SharePoint Server.

**Шаблонът на сайта не може да бъде създаден или не работи правилно**

Може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) на шаблона и да не се активира. Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона на сайта, за да създадете сайт.

- Проверете дали някои списъци или библиотеки надхвърлят [прага за ограничаване на списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) на 5000 елемента, тъй като това може да блокира създаването на шаблон на сайт.

- Сайтът може да използва твърде много ресурси и следователно шаблонът на сайта надвишава ограничението от 50 МБ.


- Има проблеми с показването на данни от списък, който използва справочна колона. За повече информация вижте [шаблон генериран списък не показва данни от правилния списък за търсене в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

За по-подробна информация относно често срещани проблеми и решения, моля, проверете [Създаване и използване на шаблони за сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



