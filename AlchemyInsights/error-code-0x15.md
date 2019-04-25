---
title: Код на грешка 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър.
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402728"
---
Ако получавате грешка докато активиране офис 2013 на отдалечен работен плот услуги (RDS) внедрявания, помислете за разрешаването на ADAL чрез редактиране на системния регистър. 
  
|**Ключ на системния регистър**|**Тип**|**Стойност**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
За повече информация вижте [Разрешаване модерни удостоверяване за офис 2013 на Windows устройства](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ЛОТАРИНГИЯ е активирана по подразбиране в Office 365 подпора и офис 2016. > отдалечен работен плот услуги (RDS) е предварително обявен за терминални услуги. 
  

