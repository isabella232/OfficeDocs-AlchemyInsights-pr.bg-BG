---
title: Отстраняване на неизправности при OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664987"
---
# <a name="troubleshoot-onedrive-crashes"></a>Отстраняване на неизправности при OneDrive

Ако OneDrive се срива многократно, изпробвайте тези стъпки за отстраняване на неизправности:

**Проверете дали ключовете на системния регистър не са зададени:**

1. Чрез редактора на системния регистър отидете до HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ако DisableFileSyncNGSC е наличен и зададен на 1, отворете ключа и променете стойността на 0.
3. Ръчно стартиране на OneDrive, като отидете в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение на OneDrive.

**Нулиране на OneDrive:**

Бележки

- Нулирането на OneDrive прекъсва всички ваши съществуващи връзки за синхронизиране (включително вашия личен OneDrive, ако е настроен).
- Няма да загубите файлове или данни, като нулирате OneDrive на вашия компютър.

**За нулиране на OneDrive:**

1. Отворете диалоговия прозорец за изпълнение, като натиснете клавиша Windows и R.
2. Въведете% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset и натиснете OK. За кратко може да се появи команден прозорец.
3. Ръчно стартиране на OneDrive, като отидете в "Старт" ![Натиснете клавиша Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), въведете OneDrive в полето за търсене и след това щракнете върху настолното приложение на OneDrive.

Бележки

- Ако сте избрали да синхронизирате само някои папки преди нулирането, ще трябва да направите това отново, след като синхронизирането завърши. Прочетете [Изберете кои папки на OneDrive да се синхронизират с вашия компютър](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   за повече информация.
- Ще трябва да изпълните това за своя личен OneDrive и OneDrive за бизнеса.