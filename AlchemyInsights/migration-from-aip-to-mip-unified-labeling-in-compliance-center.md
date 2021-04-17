---
title: Мигриране от AIP към MIP/единно етикетиране в центъра за съответствие
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825360"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Мигриране от AIP към MIP/единно етикетиране в центъра за съответствие

За да мигрирате от AIP етикети към единно етикети в центъра за защита и съответствие, направете следното:

**Активиране на защитата от портала на Azure**

1. Ако все още не сте го направили, отворете нов прозорец на браузъра и [влезте в портала на Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Навигирайте до **острието за защита на информацията в Azure.** Например в менюто концентратор щракнете върху **Всички услуги** и започнете да **въвеждате информация** в полето Филтър. Изберете **Защита на информацията в Azure**. Ако преди не сте осъществявали достъп до острието за защита на информацията в Azure, вижте едноличните допълнителни стъпки, [за](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) да добавите това острие към портала. За да отворите острието за защита на информацията в Azure, трябва да имате план [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) или план на Office 365, който включва управление на правата. Ако имате един от тези абонаменти, но видите съобщение, че не може да бъде намерен валиден абонамент, се [обърнете към поддръжката на Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или използвайте стандартните канали за поддръжка.

2. Намерете **опциите на** менюто Управление и изберете **Активиране на защитата**. Щракнете **върху Активиране** и след това потвърдете действието. Когато активирането завърши, информационната лента показва **успешното активиране.**

**Мигриране на етикети за защита на информацията на Azure към центъра за защита на Office 365 & съответствие**

1. Уверете се, че сте влезли като потребител с разрешение на глобален администратор.

2. Навигирайте до **острието за защита на информацията в Azure.**

3. От опцията **Управление** на менюто изберете **Единно етикети .**

4. В защитата **на информацията на Azure – Унифицирано острие за** етикети щракнете върху **Активиране** и следвайте онлайн инструкциите.

**Забележка:** Уверете се, че имате подходящите разрешения, преди да активирате мигрирането на центъра за & съответствие. Вижте тези статии за повече информация:

1. [Трябва ли да сте глобален администратор, за да конфигурирате защитата на информацията в Azure, или мога да делегирам на други администратори?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важна информация за административните роли след мигриране към центъра за & съответствие.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

За повече информация относно мигрирането на AIP към единно етикетиране към центъра за защита и съответствие вижте [Мигриране на етикети](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
