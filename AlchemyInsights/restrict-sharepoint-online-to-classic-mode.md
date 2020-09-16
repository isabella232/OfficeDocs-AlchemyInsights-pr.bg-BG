---
title: Ограничаване на SharePoint Online в класически режим
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751411"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Ограничаване на SharePoint Online в класически режим

Някои организации все още изискват класическа среда за работа. Макар че няма планове за премахване на класическия режим на ниво на гранули, вече не е възможно да се ограничава цяла организация (клиент) към класически режим за списъци и библиотеки.

Администраторът ще има следните опции за управление на отделни списъци и библиотеки в класически режим с помощта на гранулирани превключватели за отписване, които предоставяме на следните нива:

- колекция от сайтове
- сайт
- списък
- Библиотека

Освен това списъците, които използват определени функции и персонализации, които не се поддържат от Modern, все още ще бъдат прехвърлени автоматично в класически режим.

Началото на 1 април 2019, процесът за забраняване на отказване на ниво клиент за модерен списък и библиотеки ще започва и продължава до 31 май 2019.  Списъците и библиотеките, които са в класически режим като резултат от отписването на клиент, автоматично ще бъдат прехвърлени към модерни.

Ако имате нужда от класически режим, Вижте повече информация [тук](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) и инструкции за PNP PowerShell [тук](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , който описва опции и инструменти, които можете да използвате днес, за да използвате класическа среда за работа.
