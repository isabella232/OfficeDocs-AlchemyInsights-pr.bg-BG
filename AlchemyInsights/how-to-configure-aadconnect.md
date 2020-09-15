---
title: 646 как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704478"
---
# <a name="configure-sync-features"></a>Конфигуриране на функции за синхронизиране

Azure AD Connect включва няколко функции, които са разрешени по подразбиране, или че можете да ги разрешите по-късно. Някои функции изискват допълнителна конфигурация в определени среди.

- Ограничения за [филтриране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обектите се синхронизират с Azure ad. По подразбиране всички потребители, контакти, групи и акаунти за компютри с Windows 10 се синхронизират. Можете да включвате или изключвате обекти на базата на домейни, OU или други атрибути.

- [Синхронизиране на хеширане на парола](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизира Хеширането на парола от локалния указател Active Directory в Azure ad. Това позволява управление на паролите на едно място, но използва същата парола както в локалната среда, така и в облака. Тъй като Active Directory е авторитетен източник, можете да използвате собствените си правила за парола.

- [Услугата за самостоятелно нулиране на парола (парола)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да нулират своите собствени пароли в облака, като все пак прилагат вашите локални правила за парола.

- [Device нефиксирани](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява на регистрираните устройства в Azure ad да се изписват обратно в локалния указател Active Directory, така че да могат да бъдат използвани за условен достъп.

- [Предотвратяване на случайни изтривания](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е разрешено по подразбиране, за да се предотврати твърде много изтривания на едновременни обекти (повече от обекти на 500 за синхронизация). Можете да промените тази настройка така, че да отговаря на нуждите на вашата организация.

- [Автоматичната надстройка](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е разрешена по подразбиране за експресните инсталации и помага да се гарантира, че вашата версия на Azure ad Connect винаги е актуална.
