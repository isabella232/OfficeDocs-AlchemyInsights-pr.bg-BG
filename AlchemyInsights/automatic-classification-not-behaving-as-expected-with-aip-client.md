---
title: Автоматичната класификация не се държи по очаквания начин с AIP клиента
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
- "9002266"
- "4373"
ms.openlocfilehash: b7ab09fe8430a54dacf2cd1ba076414a5f562541
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820887"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматичната класификация не се държи по очаквания начин с AIP клиента

Автоматичната класификация не се държи според очакванията, използвайте следните препоръчителни указания:

1. Ако имате проблеми с автоматичното етикетиране, вижте Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какви типове поверителна [информация търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Проверете дали използвате правила с обхват, които не са конфигурирани правилно: Как да конфигурирате правилата за защита на информацията в Azure за определени потребители с [помощта на правилата с обхват.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
3. Ако автоматичното етикетиране не работи за Outlook при прикачване на етикетиран документ, проверете дали това не е дефинирано като описано тук: Настройки на системния регистър на `DRMEncryptProperty` [IRM за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ако сте използвали [вградените типове информация за вашите правила](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) за защита на информацията в Azure, проверете дали съдържанието ви отговаря на очаквания формат.
5. Уверете се, че етикетът е конфигуриран по подходящ начин за **Автоматично или** **Препоръчително**. (**Автоматичното** етикетиране е налично за всички приложения на Microsoft 365, докато **Препоръчва** се е налично за всички приложения на Microsoft 365 с изключение на Outlook.)
6. Не можете да използвате автоматична класификация за документи и имейли, които преди това са били ръчно етикетирани или предварително автоматично етикетирани с по-висока класификация.  За повече информация вижте: [Как се прилагат автоматичните или препоръчителните етикети.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ако все още имате проблеми, съберете регистрационните файлове на клиентите за защита на информацията в Azure и прикачете експортираните регистрационни файлове към билета за поддръжка. За да експортирате регистрационни файлове за защита на информацията в Azure:
    - Отворете документ на Office или създайте нов имейл в Outlook.
    - Щракнете **върху Помощ за защита/чувствителност** и обратна  >  **връзка.**
    - Щракнете **върху Експортиране на регистрационни файлове**.
    - Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към вашата заявка за обслужване.

За допълнителна информация вижте:

- [Как се конфигурират условията за автоматична и препоръчителна класификация за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Ръководства за "Как да" за често срещани сценарии, които използват защитата на информацията в Azure](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Преглед на абонаментите и функциите за защита на информацията в Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Изисквания за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Урок за бърз старт за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Изтегляне на клиента за защита на информацията в Azure](https://www.microsoft.com/download/details.aspx?id=53018)
