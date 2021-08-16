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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968366"
---
# <a name="changing-ews-throttling-settings"></a>Промяна на настройките за ограничаване на EWS

Изпълнете нашия автоматизиран тест, който ще ви позволи да промените правилата за ограничаване на EWS за времетраенето на мигрирането. Обърнете внимание, че дори след като това се изпълни, импортирането на EWS все още ще бъде ограничено до 150 мб на 5 минути на пощенска кутия; за да постигнете по-високи скорости на пропускателна способност за мигриране, мигрирайте повече потребители едновременно.

Обърнете внимание, че промените в правилата за ограничаване на EWS нямат ефект върху следните типове мигриране (с помощта на инструменти на Microsoft): Хибридно, cutover/Staged (RPC/HTTP), IMAP, G Suite, Публична папка или УСЛУГА за импортиране на PST.