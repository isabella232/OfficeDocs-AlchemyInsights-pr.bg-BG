---
title: Преминаване от сървърите за имена на Microsoft обратно към управлението на вашите собствени DNS записи
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506230"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Преминаване от сървърите за имена на Microsoft обратно към управлението на вашите собствени DNS записи

Преди това сте променили своите NS записи, за да сочите към Microsoft (ns1.bdm.microsoftonline.com), но сега сте решили да управлявате свои собствени DNS записи:

В уеб сайта на регистратора на домейни променете сървъра за имена обратно на вашия регистратор или предишна настройка. Ако не сте запознати с DNS, свържете се с поддръжката при регистратора на домейни. Обърнете внимание, че промените в сървъра за имена могат да отнемат до 48 часа, за да се разпространяват. 

1. В портала Microsoft 365 администратор отидете **на Настройки** домейни , поставете отметка в квадратчето до  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)домейна и изберете Управление **на DNS**. 

2. В съветника изберете Добавяне на **собствени DNS записи и** завършване на съветника. Това променя начина, по който се управлява ВАШИЯТ DNS, и след това ви позволява да добавите dns записите по избор, необходими за поддръжка на избраните от вас услуги.

Ако сте променили записите на сървърите за имена на Microsoft и имате уеб сайт, можете да добавите DNS записи за уеб сайта, вместо да променяте сървърите за имена обратно. За повече информация вижте Актуализиране на [DNS записите, за да запазите уеб сайта си при текущия си доставчик на хостинг.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


