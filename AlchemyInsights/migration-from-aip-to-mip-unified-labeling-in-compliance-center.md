---
title: Миграция от ГЛП към MIP/унифицирани етикети в центъра за съответствие
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236309"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Миграция от ГЛП към MIP/унифицирани етикети в центъра за съответствие

За да мигрирате от AIP етикети към единни етикети в центъра за защита и съответствие, направете следното:

**Активиране на защита от портала на Azure**

1. Ако още не сте го направили, отворете нов прозорец на браузъра и [влезте в портала на Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Навигирайте до острието **за защита на информацията в Azure.** Например в менюто на концентратор щракнете върху **всички услуги** и започнете да въвеждате **информация** в полето филтър . Изберете **Защита на информацията в Azure**. Ако не сте осъществили достъп до острието за защита на информацията в Azure преди, вижте еднократно [допълнителни стъпки,](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) за да добавите този нож към портала. За да отворите острието за защита на информацията в Azure, трябва да имате [или план за защита на информацията в Azure,](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) или план на Office 365, който включва управление на правата. Ако имате един от тези абонаменти, но видите съобщение, че не може да бъде намерен валиден абонамент, [се свържете с поддръжката на Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или използвайте стандартните канали за поддръжка.

2. Намерете опциите **на менюто Управление** и изберете Активиране на **защитата**. Щракнете върху **Активиране**, след което потвърдете действието си. Когато активирането завърши, информационната лента показва **активирането завърши успешно**.

**Мигриране на етикети за защита на информацията на Azure в Центъра за съответствие на & на Office 365**

1. Уверете се, че сте влезли като потребител с разрешение за глобален администратор.

2. Навигирайте до острието **за защита на информацията в Azure.**

3. От опцията **Управление на** менюто изберете **Унифицирано етикетиране**.

4. В защита на **информацията за Azure - унифицирани етикетиране** blade click **Активиране** и следвайте онлайн инструкциите.

**Забележка**: Проверете дали имате необходимите разрешения преди активиране на защитата & съответствие център миграция. Вижте тези статии за повече информация:

1. [Трябва ли да сте глобален администратор, за да конфигурирате защитата на информацията в Azure или да делегирам на други администратори?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важна информация за административни роли след мигриране на центъра за & съответствие на защитата.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

За повече информация относно мигрирането на унифициран етикет към центъра за защита и съответствие вижте [Мигриране](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)на етикети .
