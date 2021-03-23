---
title: Конфигуриране на точка на свързване на услугата (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034921"
---
# <a name="configure-service-connection-point-scp"></a>Конфигуриране на точка на свързване на услугата (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Причина**: не можете да прочетете SCP обекта и да получите информацията за клиент на Azure ad
- **Разделителна способност**: прегледайте секцията [Конфигуриране на точка на свързване на услуга](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**План за действие**

- Проверете дали устройството е получило GPO за контролираната проверка.
- Уверете се, че GPO е създал ключове от системния регистър.
- Уверете се, че имате 2 ключа, създадени със своя ИД на директорията и домейна на домейн onmicrosoft.

**Конфигуриране на настройките на системния регистър за клиент за SCP**

Използвайте примера по-долу, за да създадете обект с групови правила (GPO), за да разположите настройка на системния регистър, които конфигурират SCP запис в системния регистър на вашите устройства.

1. Отворете конзолата за управление на груповите правила и създайте нов GPO във вашия домейн.
     - Осигурете си новосъздадено име за GPO (например ClientSideSCP)

2. Редактирайте GPO и намерете следния път: **конфигурацията на компютъра > предпочитания > настройки на Windows > системен регистър**.

3. Щракнете с десния бутон върху **регистратура** и изберете **нов > елемент от системния регистър**.

4. В раздела **Общи** конфигурирайте следното:
  
- **Действие**: актуализиране
    
- **Кошер**: HKEY_LOCAL_MACHINE
    
- **Клавиш път**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Име на стойност**: TenantId
    
- **Тип стойност**: REG_SZ
    
- **Данни за стойност**: GUID или ИД на указателя на вашата инстанция на Azure ad (тази стойност може да бъде намерена в **портала на Azure > azure Active directory > свойства > ИД на директорията**)
 
- Щракнете върху **OK**.
 
5. Щракнете с десния бутон върху **регистратура** и изберете **нов > елемент от системния регистър**.

6. В раздела **Общи** конфигурирайте следното:
  
- **Действие**: актуализиране
    
- **Кошер**: HKEY_LOCAL_MACHINE
    
- **Клавиш път**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Име на стойност**: TenantName
    
- **Тип стойност**: REG_SZ
    
- **Данни за стойност**: вашето потвърдено име на домейн, ако използвате външна среда, като НАПРИМЕР AD FS. Вашите удостоверени имена на домейни или името на вашия домейн в onmicrosoft.com (например contoso. домейн onmicrosoft). com, ако използвате управлявана среда

- Щракнете върху **OK**.

7. Затворете редактора за новосъздадения GPO.

8. Свържете новосъздадения GPO до желаното място, където се съдържат домейни, които принадлежат на вашата управлявана популация за внедряване.

За повече информация вижте [управление на проверката на хибридно AZURE ad JOIN – AZURE ad | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) и  [отстраняване на неизправности в хибридни Azure Active Directory присъединен устройства | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









