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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772251"
---
# <a name="encrypt-email-messages-in-outlook"></a>Шифроване на имейл съобщения в Outlook

Шифроването на съобщения в Microsoft 365 е вградено в Microsoft Azure Rights Management (Azure RMS), който е част от защитата на Azure Information. Ако абонаментът ви включва Azure Rights Management или Azure Information Protection, не **е нужно да правите нищо, за да разрешите ръчно или да активирате** услугата за управление на правата.

Въз основа на обратната връзка от клиентите, ние вече няма да разрешаваме правилата за пощенския поток, за да Шифроваме автоматично изходящи имейли, които съдържат определен тип поверителна информация в своя клиент по подразбиране. Вместо това ще ви предоставим подробни инструкции как да направите това сами. За допълнителна информация как да създадете транспортно правило за шифроване на поверителна информация вижте [тази статия](https://aka.ms/OmeEtr).

- Ако използвате Outlook в уеб (наричан преди **OWA**): Когато съставяте имейл съобщение, просто щракнете върху **защита** в OWA. Това ще приложи разрешение "не Препращай". Щракнете върху **Промяна на разрешенията** и изберете **шифроване** , за да шифровате само съобщението.

- Ако използвате **клиент на Outlook**: за да изпратите шифровано съобщение от Outlook 2013 или 2016 или Outlook 2016 for Mac, изберете разрешения за **Опции**  >  **Permissions**, след което изберете опцията за защита, която ви е необходима.

- За да **шифровате автоматично всички имейли** , изпратени до определени получатели или външни партньорски организации, трябва да създадете правило за транспортен поток за пощенските съобщения в центъра за администриране на Exchange. Подробни инструкции се предоставят в [тази статия от поддръжката](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

