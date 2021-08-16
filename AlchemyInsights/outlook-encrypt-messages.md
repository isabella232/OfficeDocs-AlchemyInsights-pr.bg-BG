---
title: S/MIME в Outlook в уеб
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010713"
---
# <a name="encrypt-email-messages-in-outlook"></a>Шифроване на имейл съобщения в Outlook

Microsoft 365 Шифроването на съобщения е изградено на microsoft Azure Rights Management (Azure RMS), което е част от защитата на информацията в Azure. Ако абонаментът ви включва Azure Rights Management или Защитата на информацията в Azure, не е необходимо да предприемате никакви действия, за да разрешите или активирате **услугата за** управление на правата ръчно.

Въз основа на обратната връзка от клиентите повече няма да разрешаваме на Exchange на пощенския поток автоматично да шифрова изходящите имейли, съдържащи определен тип поверителна информация във вашия клиент по подразбиране. Вместо това предоставяме подробни инструкции как можете да направите това сами. За допълнителни подробности как да създадете транспортно правило за шифроване на поверителна информация вж. [тази статия.](https://aka.ms/OmeEtr)

- Ако използвате Outlook в уеб (преди **OWA**): Когато съставянето на имейл съобщение, просто щракнете върху **Защита** в OWA. Това ще приложи разрешение "Не препращай". Щракнете **върху Промяна на разрешение** и изберете **Шифроване,** за да шифровате само съобщението.

- Ако използвате **Outlook** клиент : За да изпратите шифровано съобщение от Outlook 2013 или 2016 или Outlook 2016 for Mac, изберете **Опции** разрешения , след което изберете опцията за защита,  >  от която се нуждаете.

- За **да шифровате автоматично всички** имейли, изпратени до определени получатели или организации на външни партньори, трябва да създадете транспортно правило за пощенския поток в Exchange център за администриране. Подробни инструкции са дадени в [тази статия за поддръжка.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

