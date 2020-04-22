---
title: как да импортирате-nk2-файлове
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759321"
---
# <a name="how-to-import-nk2-files"></a>Как да импортирате .nk2 файлове 

Когато стартирате Microsoft Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365 за първи път, вашият кеш за псевдоними (съхранява в име на *профил*.nk2 файл) се импортира в скрито съобщение в хранилището на съобщения по подразбиране.

За да импортирате .nk2 файлове в Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365, уверете се, че .nk2 файлът е в следната папка: %appdata%\Microsoft\Outlook

**Забележка:**.nk2 файлът трябва да има същото име като текущия ви профил в Outlook 2013 или Outlook 2016. По подразбиране името на профила е "Outlook". За да проверите името на профила, изпълнете следните стъпки: 
1. Щракнете върху **Старт**и след това щракнете върху **Контролен панел**.
2. Щракнете двукратно върху **поща**.
3. В диалоговия прозорец Настройка на пощата изберете **Показване на профили**.
4. Изберете **Стартиране на** > **изпълнение**.
5. В полето **Отвори** въведете *outlook.exe /importnk2*и след това изберете **OK**. 

След като импортирате .nk2 файла, съдържанието на файла се обединяват в съществуващите псевдоним кеш а се съхраняват в пощенската кутия.

**Забележка:**.nk2 файлът се преименува с .old разширение на файла следващия път, когато стартирате Outlook 2013, Outlook 2016, Outlook 2019 или Outlook за Microsoft 365. Ако искате да импортирате отново .nk2 файла, първо премахнете .old разширението на файла.

За повече информация [вж.](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)