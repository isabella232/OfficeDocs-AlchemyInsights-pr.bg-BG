---
title: Преминаване от ПДИ към ПМД/унифицирано етикетиране в центъра за съответствие
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674315"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Преминаване от ПДИ към ПМД/унифицирано етикетиране в центъра за съответствие

За да мигрирате от етикети на ПДИ към унифицирани етикети в центъра за защита и съответствие, направете следното:

**Активиране на защитата от портала на Azure**

1. Ако все още не сте го направили, Отворете нов прозорец на браузъра и [Влезте в портала на Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Придвижете се до ножа за **защита на информацията на Azure** . Например в менюто концентратор щракнете върху **всички услуги** и започнете да въвеждате **информация** в полето Филтър. Изберете **информация за Azure Protection**. Ако все още не сте отворили приложението Azure за защита на информацията, вижте еднократни [допълнителни стъпки](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , за да добавите това острие към портала. За да отворите инструмента за защита на информацията на Azure, трябва да имате [план на Azure за защита на информацията](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) или план на Office 365, който включва управление на правата. Ако имате един от тези абонаменти, но видите съобщение, че не може да бъде намерен валиден абонамент, [обърнете се към поддръжката на Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) или използвайте стандартните канали за поддръжка.

2. Намерете опциите за **управление** на менюто и изберете **активиране на защитата**. Щракнете върху **Активирай**и след това потвърдете действието си. Когато активирането приключи, информационната лента показва **успешното завършване на активирането**.

**Мигриране на Azure за защита на информационните етикети към центъра за администриране на & на Office 365 2010**

1. Уверете се, че сте влезли като потребител с разрешение на глобален администратор.

2. Придвижете се до ножа за **защита на информацията на Azure** .

3. От опцията **управление** на менюто изберете **обединени етикети**.

4. В центъра за **защита на информацията на Azure – унифицирано** острие за етикетиране щракнете върху **Активирай** и следвайте онлайн инструкциите.

**Забележка**: Уверете се, че имате подходящите разрешения, преди да активирате мигрирането на центъра за съответствие на защитата &. Вижте следните статии за повече информация:

1. [Трябва ли да сте глобален администратор, за да конфигурирате Azure Information Protection или мога ли да делегирам на други администратори?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важна информация за административните роли след мигриране към центъра за съответствие на & за защита.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

За повече информация относно обединената миграция на етикети към центъра за сигурност и съответствие вижте [мигриране на етикети](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
