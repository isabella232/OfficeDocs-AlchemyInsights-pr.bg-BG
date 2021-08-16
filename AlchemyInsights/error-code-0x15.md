---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка при активиране на Office 2013 в разполагания на услуги за отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100751"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Грешка при активиране на Office 2013 на услуги за отдалечен работен плот

Ако получавате грешка при активиране на Office 2013 в разполагания на услуги за отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
  
|**Ключ от системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

За повече информация вижте Разрешаване [на модерно удостоверяване за Office 2013 на Windows устройства.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL е разрешено по подразбиране в Приложения на Microsoft 365 за предприятия и Office 2016. Услугите за отдалечен работен плот (RDS) преди това са наречени терминални услуги.
  