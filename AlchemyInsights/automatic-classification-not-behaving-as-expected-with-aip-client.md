---
title: Автоматична класификация, която не се държи според очакванията при AIP клиента
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508365"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Автоматична класификация, която не се държи според очакванията при AIP клиента

Автоматичната класификация не се държи според очакванията, използвайте следните препоръчителни насоки:

1. Ако имате проблеми с автоматичното етикетиране, вижте [Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какво се търси [типовете поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Проверете дали използвате обхват правила, които не са конфигурирани правилно: [как да конфигурирате правилата за защита на информация за конкретен потребител с помощта на правила с обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Ако автоматичното етикетиране не работи за Outlook при прикачване на документ с етикет, проверете това `DRMEncryptProperty` не е дефинирано, както е описано тук: [IRM настройки на системния регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Ако сте използвали [вградените типове информация](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) за правилата за защита на информацията в Azure, проверете дали съдържанието ви съответства на очаквания формат.
5. Проверете дали етикетът е конфигуриран правилно за **автоматично** или **препоръчително**. (**Автоматичното** етикетиране е налично за всички приложения на Office, докато **препоръчва се** за всички приложения на Office, с изключение на Outlook.)
6. Не можете да използвате автоматична класификация за документи и имейли, които преди това са били ръчно етикетирани или автоматично етикетирани с по-висока класификация.  За повече информация [вж.](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)
7. Ако все още имате проблеми, събира Azure информация защита клиентски регистрационни файлове и приложете експортираните регистрационни файлове към вашия билет за поддръжка. За да експортирате регистрационните файлове за защита на информацията в Azure:
    - Отворете документ на Office или създайте нов имейл в Outlook.
    - Щракнете върху **Защита/Помощ за чувствителност**  >  **и обратна връзка**.
    - Щракнете върху **Експортиране на регистрационни файлове**.
    - Запишете регистрационните файлове на Ваш избор на местоположение и ги прикачете към заявката си за обслужване.

За допълнителна информация вижте:

- [Как да конфигурирате условия за автоматична и препоръчителна класификация за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Как да се водят за често срещани сценарии, които използват azure информация за защита](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Преглед на абонаментите и функциите за защита на информацията в Azure](https://azure.microsoft.com/pricing/details/information-protection)
- [Изисквания за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Ръководство за бърз старт за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Изтегляне на клиент за защита на информацията в Azure](https://www.microsoft.com/download/details.aspx?id=53018)
