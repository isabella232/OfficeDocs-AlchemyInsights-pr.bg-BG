---
title: Създаване на сайт в SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732201"
---
# <a name="create-sharepoint-sites-using-templates"></a>Създаване на сайтове на SharePoint с помощта на шаблони

Възможността за записване на сайт като шаблон не се поддържа със съвременните комуникационни или екипни сайтове. За повече информация относно използването на шаблони вижте [записване, изтегляне и качване на сайт на SharePoint като шаблон](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ето някои често срещани проблеми/решения относно записването на сайт или списък като шаблон в SharePoint online. 

**Бутонът "записване на шаблон на сайт/списък" не е наличен или липсва**

Администраторите ще трябва да разрешат скриптовете по избор да разрешат функциите на шаблона. За подробни стъпки, примери и съображения вижте 

- [Разрешаване или забраняване на скрипт по избор](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Командата Запиши сайта като шаблон не се поддържа и може да доведе до проблеми в сайтовете, които използват инфраструктурата за публикуване на SharePoint Server.

**Шаблонът за сайт не може да бъде създаден или не работи правилно**

Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и няма да се активира. Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона за сайт, за да създадете сайт.

- Проверете дали някакви списъци или библиотеки не надвишават [прага на списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) на елементите на 5000, тъй като това може да блокира създаването на шаблон за сайт.

- Сайтът може да използва твърде много ресурси и следователно шаблонът на сайта надвишава ограничението за 50 МБ.


- Има проблеми при показване на данни от списък, който използва колоната за справки. За повече информация вижте [списък, генериран от шаблон, не показва данни от правилния справочен списък в SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

За по-подробна информация относно често срещаните проблеми и решения вижте [Създаване и използване на шаблони за сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



