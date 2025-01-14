---
title: Създаване и управление на етикети или групи на устройства
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731286"
---
# <a name="create-and-manage-device-tags-or-groups"></a>Създаване и управление на етикети или групи на устройства

Добавете етикети на устройства, за да създадете логическа принадлежност към група. Етикетите на устройства поддържат правилно съпоставяне на мрежата, което ви позволява да прикачвате различни етикети, за да заснемете контекста и да разрешите динамичното създаване на списъци като част от инцидент. Етикетите могат да се използват като филтър в списен изглед "Устройства" или за групиране на устройства. За повече информация относно групирането на устройства вижте [Създаване и управление на етикети на устройства](/microsoft-365/security/defender-endpoint/machine-tags).

Можете да добавите етикети на устройства чрез:

- Използване на портала

- Задаване на стойност на ключ от системния регистър
 
**Забележка:** Възможно е да има закъснение между времето, когато етикетът се добавя към устройство и наличността му в списъка с устройства и страницата на устройството.

За да добавите етикети на устройства с помощта на API, вижте [Добавяне или премахване на API за етикети на устройства](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).

## <a name="add-and-manage-device-tags-using-the-portal"></a>Добавяне и управление на етикети на устройства с помощта на портала

1. Изберете устройството, на което искате да управлявате етикетите. Можете да изберете или да потърсите устройство от някой от следните изгледи:

    - **Табло за операции за защита** Изберете името на устройството от раздела Най-добрите устройства с активни известия.
    - **Опашка с предупреждения** – Изберете името на устройството до иконата на устройството от опашката с предупреждения.
    - **Списък с устройства** – Изберете името на устройството от списъка с устройства.
    - **Поле за** търсене – Изберете Устройство от падащото меню и въведете името на устройството.

    Можете също да стигнете до страницата за известяване чрез изгледите на файлове и IP адреси.

1. Изберете **Управление на етикетите** от реда с действия за отговор.

1. Въведете, за да намерите или създадете етикети.

Етикетите се добавят към изгледа на устройство и се отразяват в изгледа на списъка Устройства. След това можете да използвате филтъра етикети, за да видите съответния списък с устройства.

За повече информация вижте Създаване [и управление на етикети на устройства](/microsoft-365/security/defender-endpoint/machine-tags).