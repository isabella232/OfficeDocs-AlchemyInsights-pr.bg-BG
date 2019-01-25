---
title: 1554 Winsock грешка 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458373"
---
# <a name="winsock-error-10061"></a>Winsock грешка 10061

Този код на грешка означава, че Office 365 не можа да установи TCP сокет (връзка) с хост. Най-вероятната причина за тази грешка е проблем с конфигурацията на защитната стена. За да коригирате проблема, проверете следните настройки:
  
- Проверете вашата защитна стена конфигурация с информацията в [Office 365 URL и IP адреси](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Ако грешката е специфичен за Exchange онлайн защита (EOP), вие трябва да са били оповестени до промяна на [Exchange онлайн защита IP адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Уверете се, че вашият интернет доставчик (ISP) не блокира пристанището.
    
- Проверете смарт хоста и целевия сървър настройките във вашата конектори.
    
Обърнете внимание, че Office 365 не блокира *входящите* връзки по този начин. 
  

