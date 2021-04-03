---
title: Диспечер на EndPoint – Базови линии за защита
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440864"
---
# <a name="endpoint-manager---security-baselines"></a>Диспечер на EndPoint – Базови линии за защита

Базовите линии за защита са предварително конфигурирани групи от настройки на Windows, които ви помагат да приложите настройките за защита, препоръчани от съответните екипи за защита. Тези базови линии могат да бъдат персонализирани, за да предоставят само желаните настройки и стойности. За повече информация относно базовите линии на защитата вж. [Използване на базови линии за защита за конфигуриране на устройства с Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

В момента има базови линии за тези продукти:

- Настройки за защита на Windows MDM
- Защита за Microsoft Defender за крайна точка
- Microsoft Edge

Всяка от базовите линии се актуализира периодично и се издава в постъпкови версии. Всяка версия добавя и/или премахва настройки от предишната версия, за да гарантира, че базовата линия отговаря на текущите указания. Конзолата за базова линия на защита в защитата на Endpoint позволява да се сравняват различни версии, като прави промените от версия към версия видими.

За указания как най-ефективно да промените коя версия на базова линия е разположена, вижте [Управление на профилите на базови линии на защита в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

След разполагането на базова линия на защита можете да следите състоянието на разполагане и да преглеждате настройките „устройство по устройство“.

**Забележка:** Възможно е да са необходими до 24 часа, за да се покажат данните за отчитане на базови линии – от първоначалното разполагане до устройство и до 6 часа за по-нататъшни актуализации. 

Най-често срещаната причина за неприложимата настройка на базова линия е, защото същата настройка се използва в друг профил. Този сценарий може да бъде изследван за конкретно устройство, като се избере това устройство от възела „Състояние на устройството“ на профила „Базова линия на защита“. За подробности вж. [Разрешаване на конфликти за базови линии на защита](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).