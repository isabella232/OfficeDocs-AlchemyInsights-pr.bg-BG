---
title: Автоматичната класификация не се държи по очаквания начин в клиента на ПДИ
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
- "9002266"
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715190"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматичната класификация не се държи по очаквания начин в клиента на ПДИ

Автоматичната класификация не се държи според очакванията, използвайте следните Препоръчителни указания:

1. Ако имате проблеми с автоматичното етикетиране, вижте [как да конфигурирате условия за автоматична и Препоръчителна класификация за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и [за какво се търсят типовете чувствителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Проверете дали използвате правила за обхват, които не са конфигурирани правилно: [как да конфигурирате Azure Policy Protection за определени потребители, като използвате правила за обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ако автоматичното етикетиране не работи за Outlook при прикачването на документ с етикети, се уверете, че `DRMEncryptProperty` не е дефиниран като описан тук: [Настройки на IRM регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ако сте използвали [вградените типове информация](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) за правилата за защита на вашата информация за Azure, се уверете, че съдържанието съвпада с очаквания формат.
5. Уверете се, че етикетът е подходящо конфигуриран за **автоматични** или **Препоръчителни**. (**Автоматичното** етикетиране е достъпно за всички приложения на Microsoft 365, докато **препоръчването** е достъпно за всички приложения на Microsoft 365, с изключение на Outlook.)
6. Не можете да използвате Автоматична класификация за документи и имейли, които преди това са били ръчно означени или преди това са били етикетирани автоматично с по-голяма класификация.  За повече информация вижте: [как се прилагат автоматичните или препоръчваните етикети](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Ако все още имате проблеми, моля, съберете регистрите на клиентите на Azure за защита на информацията и прикачете експортираните регистрационни файлове към своя билет за поддръжка. За да експортирате регистри на Azure за защита на информацията:
    - Отворете документ на Office или създайте ново имейл съобщение в Outlook.
    - Щракнете **Protect/Sensitivity**върху  >  **помощ и обратна връзка**за защита/чувствителност.
    - Щракнете върху **експортиране на регистрационни файлове**.
    - Запишете регистрационните файлове по ваш избор и ги прикачете към вашата заявка за обслужване.

За допълнителна информация вж.:

- [Как се конфигурират условия за автоматична и Препоръчителна класификация за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Ръководство "как да" за често срещани сценарии, които използват Azure Information Protection](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Преглед на документацията за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Преглед на абонаменти и функции за защита на информацията в Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Изисквания за информация за Azure Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Ръководство за бърз старт за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Изтегляне на Azure за защита на информацията за клиента](https://www.microsoft.com/download/details.aspx?id=53018)
