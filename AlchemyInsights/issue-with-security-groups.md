---
title: Проблем със защитни групи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177367"
---
# <a name="issue-with-security-groups"></a>Проблем със защитни групи

**Ако получавате съобщение за грешка в мрежата AADDS104**

Невалидни правила за мрежова защита са най-честата причина за грешки в мрежата за Domain Services Azure Active Directory (AD DS). Групата за мрежова защита за виртуалната мрежа трябва да позволява достъп до определени портове и протоколи. Ако тези портове са блокирани, платформата Azure не може да следи или актуализира управлявания домейн. Синхронизацията между Azure AD и Azure AD DS също е повлияна. Уверете се, че сте отворили портовете по подразбиране, за да избегнете прекъсване на услугата.

За да разберете и да коригирате често срещани предупреждения за проблеми с конфигурацията на мрежата за мрежова защита, вижте [Добавяне и проверка на групи за защита](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).
