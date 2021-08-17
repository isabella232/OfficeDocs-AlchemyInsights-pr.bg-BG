---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043195"
---
# <a name="how-to-import-nk2-files"></a>Как се импортират .nk2 файлове 

Когато стартирате Microsoft Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365 за първи път, кешът за псевдоними (съхранен в файла *с* име на профил .nk2) се импортира в скрито съобщение във вашето хранилище за съобщения по подразбиране.

За да импортирате .nk2 файлове в Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365, уверете се, че .nk2 файлът е в следната папка: %appdata%\Microsoft\Outlook

**Забележка:** Файлът .nk2 трябва да има същото име като текущото Outlook 2013 или Outlook 2016. По подразбиране името на профила е "Outlook". За да проверите името на профила, изпълнете следните стъпки: 
1. Щракнете **върху Старт** и след това върху **Контролен панел**.
2. Щракнете двукратно върху **Поща**.
3. В диалоговия прозорец Настройка на поща изберете **Покажи профилите**.
4. Изберете **Стартиране на**  >  **изпълнение**.
5. В полето **Отвори** въведете *outlook.exe /importnk2* и след това изберете **OK**. 

След като импортирате .nk2 файла, съдържанието на файла се обединява в съществуващия кеш за псевдоними, съхранен в пощенската ви кутия.

**Забележка:**.nk2 файлът се преименува с разширение на .old файл при следващото стартиране на Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365. Ако искате да импортирате отново .nk2 файла, първо премахнете файловото разширение .old.

За повече информация вижте Импортиране [или копиране на списъка за автоматично довършете на друг компютър.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)