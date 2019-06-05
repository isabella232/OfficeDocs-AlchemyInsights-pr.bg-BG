---
title: Нива на разрешение на SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716881"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer проблеми с връзката 

<p>Ако SharePoint Designer изпитва проблеми с връзката до сайтове на SharePoint, харесвам опитвам следните общи решения.</p> <p><strong>Стъпка 1:</strong> <strong>Провери SharePoint Designer се актуализира&nbsp; </strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">Актуализация за SharePoint Designer 2013 (KB3114721)</a></li> </ul> <p><strong>Стъпка 2:</strong> <strong>Изчистване на локални файлове кеш</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">Затворете SharePoint Designer 2013.&nbsp;</li> <li style="font-weight: 400;">На локалния компютър преминете към следните папки да премахнете кеширани файлове.&nbsp;</li> <li style="font-weight: 400;">Щракнете върху <strong>Старт -&gt; тичам</strong> и изтрийте всички файлове, намерени под всеки от по-долу места.&nbsp;<br /><br />%APPDATA%\Microsoft\Web сървър Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">Отворете SharePoint Designer 2013 и въведете акаунта отново, за да видим дали тя работи.</li> </ol> <p><strong>Стъпка 3:</strong> <a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"> <strong>Разрешите модерни удостоверяване офис 2013 на Windows устройства</strong></a>&nbsp;</p> <p><strong>Стъпка 4:</strong> <strong>Администратори ще трябва да разрешите потребителски скрипт да позволите на SharePoint Designer връзка</strong>.</p> <p>За подробни стъпки, примери и съображения вижте <a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Разрешаване или предотвратяване на потребителски скрипт</a>.&nbsp;</p>


