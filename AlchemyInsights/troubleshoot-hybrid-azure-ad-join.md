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
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939260"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Отстраняване на неизправности при хибридно присъединяване към Azure AD

Силно препоръчително Уверете се, че едно устройство има достъп до крайни точки за регистриране на устройства под системния акаунт с помощта на скрипта [за свързване чрез регистриране на тестови устройства.](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)

1. Ако настройвате регистрации на устройства за първи път, не забравяйте да прегледате I[ntroduction to device management in Azure Active Directory, за](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) да научите как да получавате устройства под контрола на Azure AD.
1. Ако регистрирате устройства директно в Azure AD и ги запишете в Intune, уверете се, че сте [конфигурирали Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) и първо [сте](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) поставили лицензирането.
1. Уверете се, че сте упълномощени да извършвате операции в Azure AD и локалната AD. Само глобален администратор в Azure AD може да управлява настройките за регистрации на устройства. Освен това, ако настройвате автоматични регистрации във вашия локален Active Directory, ще трябва да сте администратор на Active Directory и AD FS (ако е приложимо).

За повече подробности относно разрешаването на [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) потенциални проблеми с хибридното съединение вижте Отстраняване на неизправности при хибридно присъединяване за настройване на хибридно присъединяване към Azure AD и управление на устройства с помощта на портала на Azure Ad, вижте Настройване на хибридни устройства, присъединени към Azure AD (локално присъединени [домейни),](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) и Управление на устройства [с помощта на портала на Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

За да разрешите често срещани проблеми с Azure Active Directory (AD), вижте ЧЗВ [за присъединяване към Хибридно присъединяване към Azure AD.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
