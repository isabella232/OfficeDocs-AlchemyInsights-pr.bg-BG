---
title: Конфигуриране и удължаване на срока на валидност на знаците
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916688"
---
# <a name="configure-and-extend-token-lifetimes"></a>Конфигуриране и удължаване на срока на валидност на знаците

Можете да укажете живота на Access, SAML или ИД маркер, издаден от платформата за самоличност на Microsoft. Можете да зададете маркери за цял живот за всички приложения във вашата организация, за приложение за много клиенти (мултиорганизация) или за определен принципал на услуга във вашата организация. За повече информация прочетете [конфигурируеми животи за маркери](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

За примери прочетете [примери за това как се конфигурират животи за маркери](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

За да научите как да конфигурирате живота и съвместимостта на маркер в Azure Active Directory B2C (Azure AD B2C), вижте [Конфигуриране на маркери в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Статията [Конфигурирай поведението на сесиите в Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) описва методите за еднократна идентификация (SSO), използвани в AZURE ad B2C, и ви помага да изберете най-подходящия метод за SSO при конфигуриране на правилата си.

**Колко дълго ще трае маркерите? Колко време важат за тях?**

Продължителността на живота на знаците е 1 час, а продължителността на сесията е 24 часа. Това означава, че ако не са правени искания за 24 часа, ще трябва да влезете отново, преди да поискате нов маркер.

> [!NOTE]
> След 30 май 2020, няма нов клиент, който да може да използва конфигурируеми правила за живот, за да конфигурира сесия и маркери за обновяване. Неодобрението ще се случи в рамките на няколко месеца след това, което означава, че ще спрем да почитаме съществуващи сеанси и обновете полицейски маркери. Все още можете да конфигурирате маркер за достъп до животите след отказа.






