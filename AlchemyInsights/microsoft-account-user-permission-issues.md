---
title: Създаване и използване на споделена пощенска кутия
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717336"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Отстраняване на проблем - потребителят не е намерен в директорията

<p>Ако потребителите получават съобщение за грешка <strong> &ldquo; &hellip;потребител може да&rsquo;т бъдат открити в директорията. Моля, опитайте отново&hellip; </strong> където видът на проблема е <strong> &ldquo;потребител не в директорията.&rdquo;</strong>, следните стъпки може да бъде завършена за да отстраните проблема.</p> <ol> <li>Осигуряване на сметка, която приема имейл покана е една и съща сметка, която се използва за да влезете в по-късно. Уверете се, че потребителят използва същата сметка да приемат покани и да влезете в сайта. <br /><br />За повече информация вижте <a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">как да управлявате псевдоними за вашия акаунт в Microsoft</a> да управлявате регистрацията в Office 365. <br /><br /></li> <li>Преминете към всеки сайт (ове), в която потребителят получава грешка. <br /><br />a. Добави <strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid=0&rdquo; </strong> (в кавички) в края на URL адреса на сайта. <br /><br />Пример: https://&lt;contoso&gt;.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />б. Изберете потребителя от списъка. <br /><br />c. Щракнете върху <strong>Премахване на потребителски разрешения от лентата</strong>. <br /><br />d. Добавяне обратно на потребителя и изпрати покани на потребителя.</li> </ol>

