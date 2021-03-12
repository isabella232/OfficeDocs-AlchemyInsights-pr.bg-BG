---
title: Коригиране на правила за клиент (отмяна на действие)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743331"
---
# <a name="fix-tenant-policy-action-override"></a>Коригиране на правила за клиент (отмяна на действие)

Политиката за анти-спам във вашия клиент е засегнала това съобщение. За да прегледате правилата, направете следното:

1. Отидете в центъра за администриране на [& на Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143)и след това отидете в раздела за правила за **управление на заплахите**  >    >  [](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Проверете дали **Източникът на правилата** указва следното:  **Add-XHeader/ModifySubject/пренасочване/изтриване/без действие/СК съобщение**

    Ако е така, в раздела по **избор** Проверете настройките за правилата, които са засегнали съобщението. Възможно е **стандартните настройки** , приложени към всички клиенти на Exchange Online Protection, да са засегнали съобщението.

За повече информация за конфигурирането на правилата за филтриране на нежелана поща вижте [Конфигуриране на правилата за филтриране на нежелана поща](https://go.microsoft.com/fwlink/?linkid=2101431).
