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
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102560"
---
# <a name="delete-or-restore-applications"></a>Изтриване или възстановяване на приложения

**За да изтриете приложение от вашия клиент на Azure AD:**

1. В **портала на Azure AD** изберете **Корпоративни приложения**. След това намерете и изберете приложението, което искате да изтриете.
2. В **секцията** Управление в левия екран изберете **Свойства**.
3. Изберете **Изтрий** и след това изберете **Да,** за да потвърдите, че искате да изтриете приложението от вашия клиент на Azure AD.

За повече информация как да изтриете приложение, вижте Бързо започване: Изтриване на приложение [от вашия клиент на Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

В PowerShell кратката команда [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) премахва конфигурациите на прокси сървър на приложение от конкретно приложение в Azure Active Directory и може да изтрие приложението напълно, ако е зададено.

Можете да **възстановите изтрито приложение с** помощта на PowerShell. След като приложението, което искате да възстановите, е идентифицирано, можете да го възстановите с [помощта на Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
