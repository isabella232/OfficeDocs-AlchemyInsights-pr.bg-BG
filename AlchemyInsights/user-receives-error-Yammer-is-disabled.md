---
title: Потребителят получава грешка AADSTS7000112 Yammer е забранена
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197748"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Потребителят получава грешка AADSTS7000112 Yammer е забранена

Ако получите грешка "AADSTS7000112: приложение"00000005-0000-0ff1-ce00-000000000000000"(Yammer) е забранена", съществува проблем с принципал на услугата в Рамките на Azure AD. Администраторът може да е забранил принципа на услугата, за да блокира достъпа до Yammer.

Забраняването на принципа на услугата не се препоръчва и може да предизвика допълнителни проблеми. За повече информация относно поддържания подход за блокиране на потребителски достъп до Yammer вижте [Изключване на достъпа на Yammer за потребители на Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

За да коригирате този проблем в Портала на Azure и възстановяване на потребителски достъп до Yammer:

1.  Отворете страницата Azure Active Directory и изберете **Корпоративни приложения** в **управление** в левия навигационен екран.
3.  Въведете **Office 365 Yammer** в полето за търсене и изберете името на приложението, за да отворите настройките.
4.  Изберете **Свойства** под **Управление** в левия навигационен екран.
5.  Задайте стойността на **разрешено за потребители да влизат в** **да**? След това изберете **Записване**.
6.  Влезте отново в Yammer. Може да се наложи да изчистите бисквитките.

Освен това изпълнете команди на PowerShell, за да зададете стойността. За повече информация вижте ["Съжаляваме, но имаме проблеми с влизането ви в" грешка, когато щракнете върху плочката Yammer в Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 