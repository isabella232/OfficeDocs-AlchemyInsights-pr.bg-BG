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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316675"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Грешка при активиране Office 2013 на услуги за отдалечен работен плот

Ако получавате грешка при активиране на Office 2013 в разполагания на услуги за отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
  
|**Ключ от системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

За повече информация вижте Разрешаване [на модерно удостоверяване за Office 2013 на Windows устройства.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Забележка:** ADAL е разрешен по подразбиране в Приложения на Microsoft 365 за предприятия и Office 2016. Услугите за отдалечен работен плот (RDS) преди това са наречени терминални услуги.
  