---
title: 932 надстройване на AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806028"
---
# <a name="upgrade-azure-ad-connect"></a>Надстройка на Azure AD Connect

По подразбиране автоматичната надстройка е разрешена за Azure AD Connect, което ще ви помогне да се уверите, че използвате най-новата версия. За да проверите настройките за автоматично надстройване, използвайте кратката команда **get-ADSyncAutoUpgrade** в Azure ad PowerShell. Кратката команда ще върне една от следните стойности:

- **Разрешена**: автоматичната надстройка е разрешена.

- **Изключен**: автоматичната надстройка е забранена.

- **Спряно**: системата вече не отговаря на условията за получаване на автоматични надстройки. Не можете да конфигурирате тази стойност; Това е зададено от системата.

За повече информация вижте [автоматично надстройване](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

За да изтеглите най-новата версия на Azure AD Connect, отидете на [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
