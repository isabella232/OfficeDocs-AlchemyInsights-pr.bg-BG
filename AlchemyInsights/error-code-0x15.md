---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка при активиране на Office 2013 на услуги за отдалечен работен плот (RDS) разполагане, помислете за разрешаване на ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703127"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Грешка при активиране на Office 2013 на услуги за отдалечен работен плот

Ако получавате грешка при активиране на Office 2013 на услуги за отдалечен работен плот (RDS) разполагане, помислете за разрешаване на ADAL чрез редактиране на системния регистър.
  
|**Ключ на системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Софтуер\Microsoft\Office\15.0\Общ\Самоличност\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

За повече информация вижте [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL е разрешена по подразбиране в Microsoft 365 приложения за предприятие и Office 2016. Услугите за отдалечен работен плот (RDS) вече са били наречени терминални услуги.
  