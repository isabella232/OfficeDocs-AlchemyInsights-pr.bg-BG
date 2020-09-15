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
description: Ако получавате съобщение за грешка по време на активирането на Office 2013 при разполагане на отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709176"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Грешка при активиране на Office 2013 в отдалечени настолни услуги

Ако получавате съобщение за грешка по време на активирането на Office 2013 при разполагане на отдалечен работен плот (RDS), обмислете разрешаването на ADAL, като редактирате системния регистър.
  
|**Ключ от системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

За повече информация вижте [Разрешаване на модерното удостоверяване за Office 2013 на устройства с Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL е разрешено по подразбиране в приложенията Microsoft 365 за Enterprise и Office 2016. Отдалечените настолни услуги (RDS) бяха предварително наименувани терминални услуги.
  