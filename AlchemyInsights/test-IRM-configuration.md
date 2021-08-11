---
title: Тестване на IRM конфигурация за нови възможности за OME
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812429"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Тестване на IRM конфигурация за нови възможности за OME

За да проверите дали вашият Microsoft 365 клиент е конфигуриран да използва нови възможности за OME, изпълнете следните кратки команди, докато [сте свързани Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Проверете IRM конфигурацията на клиента си, като изпълните `Get-IRMConfiguration` . Уверете се, че тези стойности са зададени на **True:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Като използвате вашия домейн, адрес на подател и получател, изпълнете `Test-IRMConfiguration` . Ако тестът не премине, проучайте конфигурацията на IRM.

За повече информация как да проверите конфигурацията на IRM вижте Проверка [на новата конфигурация на OME в Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).