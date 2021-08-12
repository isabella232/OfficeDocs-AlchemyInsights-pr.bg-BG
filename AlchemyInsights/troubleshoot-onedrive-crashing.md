---
title: Отстраняване на OneDrive сривове
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53920996"
---
# <a name="troubleshoot-onedrive-crashes"></a>Отстраняване на OneDrive сривове

Ако OneDrive няколко пъти се срива, изпробвайте следните стъпки за отстраняване на неизправности:

**Уверете се, че ключовете от системния регистър не са зададени:**

1. С помощта на редактора на системния регистър навигирайте до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ако DisableFileSyncNGSC е наличен и зададен на 1, отворете ключа и променете стойността на 0.
3. Ръчно стартиране OneDrive, като отивате в "Старт" ![Натиснете клавиша Windows бутон](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)въведете OneDrive в полето за търсене и след това щракнете върху OneDrive настолното приложение.

**Нулиране OneDrive:**

Бележки:

- Нулирането OneDrive прекъсне всички съществуващи връзки за синхронизиране (включително вашите лични OneDrive, ако е настроено).
- Няма да загубите файлове или данни, като нулирате OneDrive на компютъра си.

**За да нулирате OneDrive:**

1. Отворете диалоговия прозорец Изпълнение, като натиснете Windows клавиша и R.
2. Въведете %localappdata%\Microsoft\OneDrive\onedrive.exe/reset и натиснете OK. За кратко може да се покаже команден прозорец.
3. Ръчно стартиране OneDrive, като отивате в "Старт" ![Натиснете клавиша Windows бутон](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)въведете OneDrive в полето за търсене и след това щракнете върху OneDrive настолното приложение.

Бележки:

- Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизирането завърши. Прочетете [Изберете кои OneDrive за синхронизиране с вашия компютър](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)за повече   информация.
- Ще трябва да попълните това за вашите лични OneDrive и OneDrive за бизнеса.