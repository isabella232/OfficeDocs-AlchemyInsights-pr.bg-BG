---
title: Виртуален конфигурационен с услуги за домейн на пад
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884858"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Виртуален конфигурационен с услуги за домейн на пад

Виртуалното конфигуриране с услугите за домейн на пад включва следните стъпки: 

1. Проверка на изправността на вашия домейн в портала на Azure https://aka.ms/aadds-health
2. Проверяване на вашия ГЯД за правила, които блокират портове, необходими за синхронизиране в Azure AD Domain Services в портала https://aka.ms/aadds-networking
3. Гарантиране, че вашата виртуална мрежа е разположена в същия Azure регион като управлявания домейн на Azure AD Domain Services.
4. Гарантиране, че нямате съществуващ домейн със същото име на домейн, което се предлага във виртуалната мрежа.

За повече информация относно проектните обмисляния във виртуалната мрежа на Azure за поддръжка на услугите за домейни на пад вижте [разглеждане на виртуални мрежи](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

