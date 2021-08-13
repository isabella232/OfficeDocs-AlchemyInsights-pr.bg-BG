---
title: Microsoft Edge на потребителски агент (настолен)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003862"
- "6914"
ms.openlocfilehash: 9311f17298fff3fee3282fe05bd1ddcd02780a80097e86b29d56ffd575a9a571
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975990"
---
# <a name="microsoft-edge-user-agent-string-desktop"></a>Microsoft Edge на потребителски агент (настолен)

Низовете на потребителски агент (UA) могат да се използват за откриване на коя версия на конкретен браузър се използва в определена операционна система. Подобно на други браузъри, Microsoft Edge тази информация в HTTP заглавката "Агент на потребител" винаги когато прави искане към сайт. Информацията за версията на браузъра може да се получи и чрез JavaScript, като се запита стойността на "navigator.userAgent".

Препоръчваме уеб разработчиците да използват функцията за откриване, когато е възможно, за да подобрят поддържането на код, да намалят уязвимостта на кода и да премахнат риска от счупване на код в случай на бъдещи актуализации на низа на UA.

За повече информация вж. [Microsoft Edge потребителски агент (настолен)](https://docs.microsoft.com/microsoft-edge/web-platform/user-agent-string).