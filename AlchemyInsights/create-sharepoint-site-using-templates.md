---
title: Създаване на сайт в SharePoint Online
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
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770412"
---
# <a name="create-sharepoint-sites-using-templates"></a>Създаване на сайтове на SharePoint с помощта на шаблони

Възможността за записване на сайт като шаблон не се поддържа от модерна комуникация или team sites. За повече информация относно използването на шаблони вижте [Записване, изтегляне и качване на сайт на SharePoint като шаблон](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ето някои често срещани проблеми/решения относно Записване на сайт или списък като шаблон в Sharepoint Online. 

**Бутонът за запазване на шаблона за сайт/списък не е наличен или липсващ**

Администраторите ще трябва да позволи персонализиран скрипт, за да активирате функциите на шаблона. За подробни стъпки, примери и съображения вж. 

- [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Запиши сайта като шаблон командата не се поддържа и може да предизвика проблеми на сайтове, които използват sharePoint Server публикуване инфраструктура.

**Шаблонът на сайта не може да бъде създаден или не работи правилно**

Шаблонът може да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и не се активира. Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона на сайта за създаване на сайт.

- Проверете дали списъците или библиотеките надвишават прага на ограничението за [списъчен изглед](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) от 5000 елемента, тъй като това може да блокира създаването на шаблон на сайт.

- Сайтът може да използва твърде много ресурси и затова шаблонът на сайта надвишава ограничението от 50 МБ.


- Има проблеми при показването на данни от списък, който използва справочна колона. За повече информация вижте [шаблон генерирани списък не показва данни от правилния списък](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)за търсене в SharePoint Online .

За по-подробна информация относно често срещаните проблеми и решения, моля, проверете [Създаване и използване на шаблони на сайтове](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



