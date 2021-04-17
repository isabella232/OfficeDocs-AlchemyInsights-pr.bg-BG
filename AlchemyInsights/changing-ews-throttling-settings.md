---
title: Промяна на настройките за ограничаване на EWS
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818025"
---
# <a name="changing-ews-throttling-settings"></a>Промяна на настройките за ограничаване на EWS

Изпълнете нашия автоматизиран тест, който ще ви позволи да промените правилата за ограничаване на EWS за времетраенето на мигрирането. Обърнете внимание, че дори след като това се изпълни, импортирането на EWS все още ще бъде ограничено до 150 мб на 5 минути на пощенска кутия; за да постигнете по-високи скорости на пропускателна способност за мигриране, мигрирайте повече потребители едновременно.

Обърнете внимание, че промените в правилата за ограничаване на EWS нямат ефект върху следните типове мигриране (с помощта на инструменти на Microsoft): Хибридно, cutover/Staged (RPC/HTTP), IMAP, G Suite, Публична папка или УСЛУГА за импортиране на PST.