---
title: 932 надстройване на AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766482"
---
# <a name="upgrade-azure-ad-connect"></a>Надграждане Azure AD свързване

По подразбиране автоматичното надстройване е разрешено за свързване с Azure AD, което помага да се гарантира, че изпълнявате най-новата версия. За да проверите настройките за автоматично надграждане, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure AD PowerShell. Кратката команда ще върне една от следните стойности:

- **Разрешено:** Автоматичното надстройване е разрешено.

- **Забранено:** Автоматичното надстройване е забранено.

- **Временно:** Системата вече не отговаря на условията за автоматично надстройване. Не можете да конфигурирате тази стойност; тя е зададена от системата.

За повече информация вижте [Автоматично надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

За да изтеглите най-новата версия [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)на Azure AD connect, отидете на .
