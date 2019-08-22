---
title: 932 надстройка AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: ff3f74348599788edd8ce0991fe49bb6a54b55af
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506072"
---
# <a name="upgrade-azure-ad-connect"></a>Свързване на ъпгрейд лазурно АД

По подразбиране автоматичен ъпгрейд е разрешена за Azure АД свържете, която помага да се гарантира, че работите най-новата версия. За да проверите настройките за автоматично ъпгрейд, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure АД PowerShell. Кратката команда ще върне един от следните стойности:

- **Активирана**: автоматичен ъпгрейд е разрешено.

- **Забранени**: автоматичен ъпгрейд е забранено.

- **Окачени**: системата вече има право да получава автоматично ъпгрейди. Не можете да конфигурирате тази стойност; Тя се определя от системата.

За повече информация вижте [автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

За да изтеглите последната версия на Azure АД се свърже, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
