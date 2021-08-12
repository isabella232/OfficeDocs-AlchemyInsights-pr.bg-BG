---
title: 646 Как да конфигурирате AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963632"
---
# <a name="configure-sync-features"></a>Конфигуриране на функции за синхронизиране

Azure AD Свързване няколко функции, които са разрешени по подразбиране или които можете да разрешите по-късно. Някои функции изискват допълнителна конфигурация в определени среди.

- [Филтрирането ограничава](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) обектите да се синхронизират с Azure AD. По подразбиране всички потребители, контакти, групи и Windows 10 се синхронизират. Можете да включвате или изключвате обекти въз основа на домейни, US или други атрибути.

- [Синхронизирането на хашовете](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) на пароли синхронизира хашта на паролата от локалния Active Directory с Azure AD. Това позволява управление на пароли в едно местоположение, но използването на една и съща парола както в локална, така и в среда в облака. Тъй като Active Directory е авторитетния източник, можете да използвате собствените си правила за пароли.

- [Самостоятелното нулиране на пароли (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да нулират собствените си пароли в облака, като все още прилагат вашите локални правила за пароли.

- [Отписване на](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) устройства позволява регистрираните устройства в Azure AD да се записват обратно в локалния Active Directory, така че да могат да се използват за условен достъп.

- [Предотвратяването на случайни изтривания](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е разрешено по подразбиране, за да се предотврати твърде много едновременни изтривания на обекти (повече от 500 обекта за синхронизиране). Можете да промените тази настройка така, че да отговаря на нуждите на вашата организация.

- [Автоматичното надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е разрешено по подразбиране за експресни инсталации и помага да се гарантира, че вашата версия на Azure AD Свързване винаги е актуална.
