---
title: Изтриване на Teams личен канал
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 33bf8a5cdc3a8e8da78c9d02e11387a778a7acce483e4485f595d9e05b344433
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948260"
---
# <a name="delete-a-teams-private-channel"></a>Изтриване на Teams личен канал

Microsoft е наясно с проблем с изтриването на Teams канал, ако имате разрешени SharePoint за съхранение за базовия SharePoint сайт. Microsoft работи по корекция. Междувременно можете да използвате следните заобиколни решения, за да изтриете частния канал.

**Изключете колекцията екип/сайт от правилата за съхранение на Sharepoint.**

1. Отидете в портала Office 365 администратор и изберете **Покажи всички** в левия навигационен екран.
2. Под **Центрове за администриране отидете на** Правила за защита & **защита** от загуба на данни  >  **за**  >  **съответствие.**
3. Идентифицирайте всички правила, които се прилагат към сайтове на Sharepoint, и променете правилата, така че сайтът на Sharepoint за екипа, съдържащ частния канал, да не е включен в правилата за съхранение.
4. Запишете правилата.
    Може да отнеме до 24 часа, за да в сила настройките на правилата.
    След като сайтът бъде изключен, можете да изтриете частния канал.  
    
Възможно ***е*** да можете да изтриете частния канал, като използвате Microsoft Teams на устройството си с Android. 

За свързана SharePoint информация вижте [Не можете да изтривате елементи в SharePoint онлайн или OneDrive за бизнеса](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).