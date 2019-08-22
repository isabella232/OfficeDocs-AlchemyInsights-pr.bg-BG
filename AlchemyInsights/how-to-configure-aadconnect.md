---
title: 646 как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 316d7253494c55a9bc94797d493897c2ddec516c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541574"
---
# <a name="configure-sync-features"></a>Конфигуриране на функции в синхронизиране

Лазурно АД свързване включва няколко функции, които са разрешени по подразбиране, или че можете да активирате по-късно. Някои функции изискват допълнителна конфигурация в специфични среди.

- [Филтрирането](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) граници обектите се синхронизират в лазурно АД. По подразбиране, всички потребители, контакти, групи и Windows 10 Компютърни акаунти са синхронизирани. Можете да включват или изключват обекти, базирани на домейни, OU или други атрибути.

- [Парола кълцам синхронизиране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизира парола кълцам от локалната Active Directory към лазурните реклама. Това позволява управление на парола в едно място, но използването на една и съща парола в двете локални и облак среди. Тъй като Active Directory е достоверният източник, можете да използвате своя собствена парола политика.

- [Самообслужване парола проучване (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да сменят паролите си собствени в облака, докато все още се прилага вашата локалната парола политика.

- [Writeback определителен устройство](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява регистрирани устройства в лазурно Рекламата да се запише обратно в локалната Active Directory, така че те могат да бъдат използвани за условен достъп.

- [Предотвратяване на случайно изтриване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е активирана по подразбиране за да се предотврати прекалено много едновременни обект делеции (повече от 500 обекта за синхронизация). Можете да промените тази настройка, за да отговори на нуждите на вашата организация.

- [Автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е активирана по подразбиране за Експресно инсталации и помага да се гарантира вашата версия на Azure АД свържете е винаги актуална.
