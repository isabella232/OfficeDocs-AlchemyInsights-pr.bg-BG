---
title: 'ОИП: Политики, които не се държат според очакванията'
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
- "4780"
ms.openlocfilehash: 91308850c06485bdd11e81bd130770aefb247118
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580754"
---
# <a name="aip-policies-not-behaving-as-expected"></a>ОИП: Политики, които не се държат според очакванията

Защита на информацията за Azure: правила не се държи според очакванията, вижте следните указания за препоръчителни указания за различни проблеми с правилата:

1. Ако имате проблеми с визуални маркировки, моля, прегледайте [Когато се прилагат визуални маркировки.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ако имате проблеми с автоматичното етикетиране, прегледайте [Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какви типове чувствителна информация [търсите](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ако имате проблеми със защитата native/Pfile, прегледайте [конфигурацията на API на файла](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Проверете дали използвате обхват правила, които не са конфигурирани правилно: [как да конфигурирате правилата за защита на информация за конкретен потребител с помощта на правила с обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ако автоматичното етикетиране не работи за Outlook прикачване на етикетиран документ, проверете дали DRMEncryptProperty не е дефиниран както е описано тук: [IRM настройки на системния регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ако все още имате проблеми, събира Azure информация защита клиентски регистрационни файлове и приложете експортираните регистрационни файлове на този билет.

1. Отворете документ на Office или създайте нов имейл в Outlook.
2. Щракнете върху **Защита/Помощ за чувствителност**  >  **и обратна връзка**.
3. Щракнете върху **Експортиране на регистрационни файлове**.
4. Запишете регистрационните файлове на ваш избор на местоположение и ги прикачете към тази заявка за услуга.

Допълнителни ресурси:

- [Как да конфигурирате етикет за визуални маркировки за Azure информация за защита](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Използване на етикети за чувствителност в приложения на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

