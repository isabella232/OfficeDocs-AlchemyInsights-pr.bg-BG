---
title: 646 Как да конфигурирате AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722516"
---
# <a name="configure-sync-features"></a>Конфигуриране на функциите за синхронизиране

Azure AD свързване включва няколко функции, които са разрешени по подразбиране или можете да разрешите по-късно. Някои функции изискват допълнителна конфигурация в определени среди.

- [Филтриране](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) граници обекти са синхронизирани Azure AD. По подразбиране се синхронизират всички потребители, контакти, групи и акаунти на компютъра в Windows 10. Можете да включите или изключите обекти на базата на домейни, ous или други атрибути.

- [Парола хеш синхронизация](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) синхронизира паролата хеш от локалната Active Directory azure AD. Това позволява управление на пароли на едно място, но използването на една и съща парола както в локалните, така и в облачните среди. Тъй като Active Directory е авторитетен източник, можете да използвате вашите собствени правила за парола.

- [Самостоятелно нулиране на паролата (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) позволява на потребителите да нулират собствените си пароли в облака, като все още прилагат правилата за локална парола.

- [Устройство с отпиване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) позволява регистрирани те да бъдат записани в Azure AD да бъдат записани обратно в локалната Active Directory, така че те могат да се използват за условен достъп.

- [Предотвратяване на случайни изтривания](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) е разрешена по подразбиране да предотврати твърде много едновременни обекти изтривания (повече от 500 обекти за синхронизация). Можете да промените тази настройка, за да отговаря на нуждите на вашата организация.

- [Автоматичното надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) е активирано по подразбиране за експресни инсталации и помага да се гарантира, че вашата версия на Azure AD Connect е винаги актуална.
