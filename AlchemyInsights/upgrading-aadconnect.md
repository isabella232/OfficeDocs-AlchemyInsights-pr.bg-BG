---
title: 932 Надстройване на AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104801"
---
# <a name="upgrade-azure-ad-connect"></a>Надстройване на Azure AD Свързване

По подразбиране автоматичното надстройване е разрешено за azure AD Свързване, което помага да се гарантира, че изпълнявате най-новата версия. За да проверите настройките за автоматична надстройка, използвайте кратката команда **Get-ADSyncAutoUpgrade** в Azure AD PowerShell. Кратката команда ще върне една от следните стойности:

- **Разрешено:** Автоматичната надстройка е разрешена.

- **Забранено:** Автоматичната надстройка е забранена.

- **Временно** преустановено: Системата вече не отговаря на условията за получаване на автоматични надстройки. Не можете да конфигурирате тази стойност; тя е зададена от системата.

За повече информация вижте Автоматична [надстройка](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

За да изтеглите най-новата версия на Azure AD Свързване, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
