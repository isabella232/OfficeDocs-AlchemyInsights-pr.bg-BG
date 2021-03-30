---
title: Отстраняване на проблеми с присъединяването към Azure AD
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404257"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Отстраняване на проблеми с присъединяването към Azure AD

1. Ако настройвате регистрации на устройства за първи път, уверете се, че сте прегледали Въведение в управлението на [устройства в Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) което ще ви напътства как да вземете Устройствата под контрола в Azure AD. 
1. Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, ще трябва да [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) се уверите, че първо сте конфигурирали [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) и че лицензирането е на първо място.
1. Уверете се, че сте упълномощени да извършвате операции в Azure AD. Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства.
1. За да направите внедряването на Azure AD присъединяване, вижте [Планиране на Azure AD Присъединяване](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

За повече подробности относно разрешаването на често срещани проблеми с присъединяването към [Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) вж. ЧЗВ за присъединяване към Azure Ad и за устройства с Windows 10 pro вижте Не може да се присъедините към компютър с Windows 10 Pro към Azure AD – трябва да [надстроите до – общност на Microsoft](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
