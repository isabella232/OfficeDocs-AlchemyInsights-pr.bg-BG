---
title: Ограничаване SharePoint онлайн до класически режим
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
ms.openlocfilehash: 6315a83ac825f96ceea60798d441de8e8e53336fe29eda4d0491dd8a6a43b352
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53958790"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Ограничаване SharePoint онлайн до класически режим

Някои организации все още изискват класическата работа в режим. Въпреки че няма планове за премахване на класически режим на гранулярно ниво, вече не е възможно да ограничите цялата организация (клиент) до класически режим за списъци и библиотеки.

Администраторът ще има следните опции за управление на отделни списъци и библиотеки в класически режим с помощта на модулни ключове за отписване, които предоставяме на следните нива:

- колекция от сайтове
- сайт
- списък
- библиотека

Освен това списъците, които използват определени функции и персонализации, които не се поддържат от модерното, ще бъдат автоматично превключени към класически режим.

От 1 април 2019 г. процесът за забраняване на отписване на нивото на клиента от модерния списък и библиотеките ще започне и ще продължи до 31 май 2019 г.  Списъците и библиотеките, които са в класически режим в резултат на отписване от клиента, автоматично ще бъдат преместени към модерни.

Ако имате нужда от класически [](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) режим, вижте повече информация тук и инструкцията за PnP Powershell [тук,](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) която описва опциите и инструментите, които можете да използвате днес, за да използвате класическата работа в режим.
