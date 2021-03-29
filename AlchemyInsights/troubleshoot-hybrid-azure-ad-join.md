---
title: Отстраняване на неизправности при хибридно присъединяване към Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401896"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Отстраняване на неизправности при хибридно присъединяване към Azure AD

Силно препоръчително Уверете се, че едно устройство има достъп до крайни точки за регистриране на устройства под системния акаунт с помощта на скрипта [за свързване чрез регистриране на тестови устройства.](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)

1. Ако настройвате регистрации на устройства за първи път, не забравяйте да прегледате I[ntroduction to device management in Azure Active Directory,](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) за да научите как да получавате устройства под контрола на Azure AD.
1. Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, уверете се, че сте [конфигурирали Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и първо [сте](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) поставили лицензирането.
1. Уверете се, че сте упълномощени да извършвате операции в Azure AD и локалната AD. Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства. Освен това, ако настройвате автоматични регистрации във вашия локален Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).

За повече подробности относно разрешаването на [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) потенциални проблеми с хибридното съединение вижте Отстраняване на неизправности при хибридно присъединяване за настройване на хибридно присъединяване към Azure AD и управление на устройства с помощта на портала на Azure Ad, вижте Настройване на хибридни устройства, присъединени към Azure AD (локално присъединени [домейни),](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) и Управление на устройства [с помощта на портала на Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

За да разрешите често срещани проблеми с присъединяването към хибриден Azure Active Directory (AD), вижте [ЧЗВ за хибридно присъединяване към Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
