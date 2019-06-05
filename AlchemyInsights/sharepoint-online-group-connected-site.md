---
title: Добавяне на група към SharePoint сайт
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719471"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>Създаване на група свързани сайт в SharePoint Online

<p><strong>Има няколко общи проблеми, срещани при създаване или повторно създаване група свързан сайт.&nbsp;</strong></p>  <p>1.Ако сте изтрили група и нейните свързани сайт и искате да създадете друг сайт със същия URL адрес, трябва да премахнете завинаги предишният сайт.</p>  <ul>  <li>Изтегли <a title="SPO управление Шел" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO управление Шел</a> - за повече информация за първи стъпки с powershell, вижте <a title="запознаване с SharePoint онлайн управление Шел" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Запознаване с SharePoint онлайн управление Шел</a>. <br /><br /></li>  <li>Премахване на сайт от изтрити сайтове използват <a title="премахване-SPODeletedSite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Премествам-SPODeletedSite</a> powershell cmdlet.</li>  </ul>  <p>Ако сте създаването на група свързани сайт и да получите предупреждение <strong>"съществува друга група със същия псевдоним вече"</strong>, проверете съществуващите групи от <a title="Office 365 от центъра за администриране на" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 от центъра за администрация на</a>. За разрешаване на проблема, изтрийте съществуващата група, ако вече не е необходимо или създадете сайт с друг псевдоним присвоени.&nbsp;</p>  <p><strong>Има различни начини за създаване и използване на съвременни групи с SharePoint.&nbsp;</strong></p>  <ol>  <li>Можете да се свържете съществуващи сайтове на Office 365 група. За повече информация, вижте <a title="свързване на Office 365 група използва SharePoint потребител ineterface" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">Свързване на Office 365 група използва SharePoint потребител ineterface</a>.</li>  <li>За да създадете свързан сайт за група на Office 365, трябва да създадете сайт на екип. За повече информация, вижте <a title="създаване на екипен сайт в SharePoint" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">Създаване на екип сайт в SharePoint.</a></li>  </ol>

