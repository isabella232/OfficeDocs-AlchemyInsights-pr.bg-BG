---
title: Изтриване или възстановяване на приложения
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014724"
---
# <a name="delete-or-restore-applications"></a>Изтриване или възстановяване на приложения

**За да изтриете приложение от своя клиент на AZURE ad**:

1. В **портала на AZURE ad** изберете **корпоративни приложения**. След това намерете и изберете приложението, което искате да изтриете.
2. В секцията **управление** в левия екран изберете **свойства**.
3. Изберете **Изтрий**, след което изберете **да** , за да потвърдите, че искате да изтриете приложението от вашия клиент на Azure ad.

За повече информация как да изтриете приложение, вижте бърз [Старт: Изтриване на приложение от клиент на Azure Active Directory (AZURE ad)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

В PowerShell командата [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) премахва конфигурациите на прокси сървър за приложения от конкретно приложение в Azure Active Directory и може да изтрие напълно приложението, ако е зададено.

Можете да **възстановите изтрито приложение** с помощта на PowerShell. След като приложението, което искате да възстановите, е идентифицирано, можете да го възстановите чрез [възстановяване на AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
