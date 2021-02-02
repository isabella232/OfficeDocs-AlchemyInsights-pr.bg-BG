---
title: Промяна на настройките за ограничаване на EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075886"
---
# <a name="changing-ews-throttling-settings"></a>Промяна на настройките за ограничаване на EWS

Моля, изпробвайте нашия автоматизиран тест, който ще ви помогне да модифицирате правилата за ограничаване на EWS за продължителността на вашата миграция. Имайте предвид, че дори след като това се изпълни, EWS вносът все още ще бъде ограничен до 150mb на 5 минути за пощенска кутия; за да постигнете по-високи скорости на пропускателна способност за мигриране, можете да мигрирате повече потребители едновременно.

Имайте предвид, че промените в правилата за ограничаване на EWS не имат ефект върху следните типове мигриране (с помощта на инструменти за Microsoft): хибридни преходна/поетапни (RPC/HTTP), IMAP, G Suite, публична папка или PST услуга за импортиране.