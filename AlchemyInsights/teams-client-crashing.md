---
title: Клиент на Teams има проблем със срив?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030516"
---
# <a name="teams-client-crashing"></a>Клиент на Teams има проблем със срив?

Ако клиентът ви в Teams има проблем със срив, опитайте следното:

- Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Уверете се, че всички [URL и диапазони от адреси за Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.

- Влезте със своя акаунт на администратор и проверете [вашето табло за изправност на услугите](https://docs.microsoft.com/office365/enterprise/view-service-health), за да проверите дали няма прекъсване или влошаване на услугата.

 - Като последна стъпка можете да се опитате да изчистите кеша на вашия клиент в Teams:

    1.  Напълно излезте от настолния клиент на Microsoft Teams. Можете да щракнете с десния бутон на мишката върху **Teams** от иконата в системната област и да щракнете върху **Изход**, или да изпълнете диспечера на задачите, за да прекратите напълно процеса.

    2.  Отидете на File Explorer и въведете %appdata%\Microsoft\teams.

    3.  След като влезете в справочния указател, ще видите няколко от следните папки:

         - От **Кеш за приложенията**, отидете на Кеш и изтрийте всеки от файловете в местоположението на кеша: %appdata%\Microsoft\teams\application cache\cache.

        - От **Blob_storage**, изтрийте всички файлове: %appdata%\Microsoft\teams\blob_storage.

        - От **Blob_storage**, изтрийте всички файлове: %appdata%\Microsoft\teams\Cache.

        - От **Бази данни**, изтрийте всички файлове: %appdata%\Microsoft\teams\databases.

        - От **GPUCache**, изтрийте всички файлове: %appdata%\Microsoft\teams\GPUcache.

        - От **IndexedDB**, изтрийте файла .db: %appdata%\Microsoft\teams\IndexedDB.

        - От **Локално място за съхранение**, изтрийте всички файлове: %appdata%\Microsoft\teams\Local Storage.

        - И накрая, от **tmp**, изтрийте всеки файл: %appdata%\Microsoft\teams\tmp.

    4. Рестартирайте своя клиент в Teams.
