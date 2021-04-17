---
title: Отстраняване на неизправности в OneDrive се срива
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826188"
---
# <a name="troubleshoot-onedrive-crashes"></a>Отстраняване на неизправности в OneDrive се срива

Ако OneDrive неколкократно се срива, изпробвайте следните стъпки за отстраняване на неизправности:

**Уверете се, че ключовете от системния регистър не са зададени:**

1. С помощта на редактора на системния регистър навигирайте до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ако DisableFileSyncNGSC е наличен и зададен на 1, отворете ключа и променете стойността на 0.
3. Ръчно стартиране на OneDrive, като отивате в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение OneDrive.

**Нулиране на OneDrive:**

Бележки:

- Нулирането на OneDrive прекъсва всички съществуващи връзки за синхронизиране (включително вашия личен OneDrive, ако е настроен).
- Няма да загубите файлове или данни, като нулирате OneDrive на компютъра си.

**За да нулирате OneDrive:**

1. Отворете диалоговия прозорец Изпълнение, като натиснете клавиша Windows и R.
2. Въведете %localappdata%\Microsoft\OneDrive\onedrive.exe/reset и натиснете OK. За кратко може да се покаже команден прозорец.
3. Ръчно стартиране на OneDrive, като отивате в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение OneDrive.

Бележки:

- Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизирането завърши. Прочетете [Изберете кои папки на OneDrive да синхронизирате с вашия компютър](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)за повече   информация.
- Ще трябва да завършите това за вашия личен OneDrive и OneDrive за бизнеса.