---
title: 932 надстройка AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389648"
---
# <a name="upgrade-azure-ad-connect"></a>Свързване на ъпгрейд лазурно АД

По подразбиране автоматичен ъпгрейд е разрешена за Azure АД свържете, която помага да се гарантира, че работите най-новата версия. За да проверите настройките за автоматично ъпгрейд, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure АД PowerShell. Кратката команда ще върне един от следните стойности: 

- **Активирана**: автоматичен ъпгрейд е разрешено.

- **Забранени**: автоматичен ъпгрейд е забранено.

- **Окачени**: системата вече има право да получава автоматично ъпгрейди. Не можете да конфигурирате тази стойност; Тя се определя от системата. 

За повече информация вижте [автоматичен ъпгрейд](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

За да изтеглите последната версия на Azure АД се свърже, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).
