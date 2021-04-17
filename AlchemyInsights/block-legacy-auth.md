---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820167"
---
# <a name="blocking-legacy-authentication"></a>Блокиране на наследено удостоверяване

Наследеното удостоверяване е израз, който препраща към искане за удостоверяване, направено от:

- По-стари клиенти на Office, които не използват модерно удостоверяване (например клиент на Office 2010).

- Всеки клиент, който използва стари пощенски протоколи, като например IMAP/SMTP/POP3.

За повече информация относно блокирането на наследено удостоверяване и разрешаването на модерно удостоверяване вижте [Блокиране на наследено удостоверяване](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).

Настройките по подразбиране за защита в Azure Active Directory (Azure AD) улесняват защитата и защитават вашата организация. Настройките за защита по подразбиране съдържат предварително конфигурирани настройки за защита за често срещани атаки.
За повече информация относно настройките за защита по подразбиране вижте [Какво са настройките по подразбиране за защита?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults). 

**Забележка:** Ако вашият клиент е създаден на или след 22 октомври 2019 г., е възможно да се сблъскате с новото поведение "защитен по подразбиране" и вече имате активирани настройки по подразбиране на защитата във вашия клиент.  В опит да защитим всички наши потребители, по подразбиране защитата се създава за всички нови клиенти, създадени.
