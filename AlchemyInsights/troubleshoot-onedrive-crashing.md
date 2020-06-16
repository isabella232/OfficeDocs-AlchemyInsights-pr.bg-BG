---
title: Отстраняване на неизправности в OneDrive сривове
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/15/2020
ms.locfileid: "44748735"
---
# <a name="troubleshoot-onedrive-crashes"></a>Отстраняване на неизправности в OneDrive сривове

Ако OneDrive многократно се срива, опитайте следните стъпки за отстраняване на неизправности:

**Уверете се, че не са зададени ключове в системния регистър:**

1. С помощта на редактора на системния регистър отидете на HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ако DisableFileSyncNGSC е наличен и е 1, отворете ключа и променете стойността на 0.
3. Ръчно стартиране на OneDrive, като отидете в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), въведете OneDrive в полето за търсене и след това щракнете върху oneDrive настолното приложение.

**Нулиране на OneDrive:**

Бележки:

- Нулирането на OneDrive прекъсва връзката между всички ваши съществуващи връзки за синхронизиране (включително вашия личен OneDrive, ако е настроен).
- Няма да загубите файлове или данни, като нулирате OneDrive на компютъра си.

**За да нулирате OneDrive:**

1. Отворете диалоговия прозорец за изпълнение, като натиснете клавиша Windows и R.
2. Въведете %localappdata%\Microsoft\OneDrive\onedrive.exe/нулиране и натиснете OK. Прозорецът на командата може да се появи за кратко.
3. Ръчно стартиране на OneDrive, като отидете в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), въведете OneDrive в полето за търсене и след това щракнете върху oneDrive настолното приложение.

Бележки:

- Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизацията приключи. Прочетете [Изберете кои папки за OneDrive да се синхронизират с компютъра ви](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)за повече   информация.
- Ще трябва да попълните това за вашия личен OneDrive и OneDrive за бизнеса.