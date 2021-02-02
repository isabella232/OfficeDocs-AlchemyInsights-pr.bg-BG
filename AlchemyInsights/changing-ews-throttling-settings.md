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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="18118-102">Промяна на настройките за ограничаване на EWS</span><span class="sxs-lookup"><span data-stu-id="18118-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="18118-103">Моля, изпробвайте нашия автоматизиран тест, който ще ви помогне да модифицирате правилата за ограничаване на EWS за продължителността на вашата миграция.</span><span class="sxs-lookup"><span data-stu-id="18118-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="18118-104">Имайте предвид, че дори след като това се изпълни, EWS вносът все още ще бъде ограничен до 150mb на 5 минути за пощенска кутия; за да постигнете по-високи скорости на пропускателна способност за мигриране, можете да мигрирате повече потребители едновременно.</span><span class="sxs-lookup"><span data-stu-id="18118-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="18118-105">Имайте предвид, че промените в правилата за ограничаване на EWS не имат ефект върху следните типове мигриране (с помощта на инструменти за Microsoft): хибридни преходна/поетапни (RPC/HTTP), IMAP, G Suite, публична папка или PST услуга за импортиране.</span><span class="sxs-lookup"><span data-stu-id="18118-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>