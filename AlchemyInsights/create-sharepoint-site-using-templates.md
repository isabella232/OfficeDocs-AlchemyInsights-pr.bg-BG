---
title: Създаване на сайт в SharePoint Онлайн
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057955"
---
# <a name="create-sharepoint-sites-using-templates"></a>Създаване SharePoint сайтове с помощта на шаблони

Възможността за записване на сайт като шаблон не се поддържа с модерни комуникации или екипни сайтове. За повече информация относно използването на шаблони вижте [Записване, изтегляне и качване на сайт на SharePoint като шаблон](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Ето някои често срещани проблеми/решения относно записването на сайт или списък като шаблон в Sharepoint Online. 

**Бутонът "Записване на шаблон за сайт/списък" не е наличен или липсва**

Администраторите ще трябва да позволят персонализирания скрипт по избор, за да разрешат функциите на шаблона. За подробни стъпки, примери и съображения вж. 

- [Разрешаване или предотвратяване на персонализиран скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Командата "Запиши сайта като шаблон" не се поддържа и може да предизвика проблеми в сайтове, които използват инфраструктурата за публикуване на SharePoint Server.

**Шаблонът за сайт не може да бъде създаден или не работи правилно**

Възможно е шаблонът да липсва [функция](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) и да не се активира. Ако функцията не е налична за активиране в текущата колекция от сайтове, не можете да използвате шаблона за сайт, за да създадете сайт.

- Проверете дали някои списъци или библиотеки [](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) надвишават граничния праг за списъчен изглед от 5000 елемента, тъй като това може да блокира създаването на шаблон за сайт.

- Сайтът може да използва твърде много ресурси и следователно шаблонът за сайт надхвърля ограничението от 50 МБ.


- Има проблеми с показването на данни от списък, който използва справочна колона. За повече информация вижте Генериран от шаблон списък не показва данни [от правилния справочен списък в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

За по-подробна информация за често срещани проблеми и решения проверете [Създаване и използване на шаблони на сайтове.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



