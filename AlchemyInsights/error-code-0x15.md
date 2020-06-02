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
description: Ако получавате грешка при активиране на Office 2013 за разполагане на услуги за отдалечен работен плот (RDS), помислете дали да разрешите ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506835"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Грешка при активиране на Office 2013 услуги за отдалечен работен плот

Ако получавате грешка при активиране на Office 2013 за разполагане на услуги за отдалечен работен плот (RDS), помислете дали да разрешите ADAL чрез редактиране на системния регистър.
  
|**Ключ на системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Софтуер\Microsoft\Office\15.0\Обща\Идентичност\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

За повече информация вижте [Разрешаване на съвременни удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL е разрешена по подразбиране в приложения на Microsoft 365 за корпоративни и Office 2016. Услугите за отдалечен работен плот (RDS) вече са били наричани терминални услуги.
  