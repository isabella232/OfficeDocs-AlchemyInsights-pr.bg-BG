---
title: Присвояване на роля на регистрационен файл за проверка в центъра за съответствие на & за защита на Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743372"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Присвояване на роля на регистрационен файл за проверка в центъра за съответствие на & за защита на Office 365

За да търсите в регистрационния файл за проверка на Office 365, на администратора трябва да е присвоена ролята на **регистрационни файлове за проверка само за преглед** или ролята на **регистрационни файлове за проверка** в Exchange Online. Тези роли се задават на ролевите групи за управление на съответствието и на организацията по подразбиране. Глобалните администратори в Office 365 и Microsoft 365 се добавят автоматично като членове на ролевата група за управление на организацията.

За да разрешите на потребителя да търси с минималното ниво на привилегии, Създайте потребителска ролева група в Exchange Online, добавете ролята за **регистрационни файлове за проверка само за преглед** или ролята на **регистрационни файлове за проверка** и след това добавете потребителя като член на новата ролева група.

За повече информация вижте [управление на ролеви групи в Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) и [търсене в регистрационния файл за проверка в центъра за съответствие на защитата &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).