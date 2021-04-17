---
title: 'AIP: Правилата не се държат според очакванията'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821616"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Правилата не се държат според очакванията

Защита на информацията в Azure: Правилата не се държат според очакванията, вижте следното за препоръчителни указания за различни проблеми с правилата:

1. Ако имате проблеми с визуалните маркировки, прегледайте [При прилагане на визуални маркировки.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ако имате проблеми с автоматичното етикетиране, прегледайте Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какво търси типовете [поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ако имате проблеми със защитата native/Pfile, прегледайте конфигурирането [на API на файл](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Проверете дали използвате правила с обхват, които не са конфигурирани правилно: Как да конфигурирате правилата за защита на информацията в Azure за определени потребители с [помощта на правилата с обхват.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Ако автоматичното етикетиране не работи за Outlook, когато прикачвате етикетиран документ, проверете дали DRMEncryptProperty не е дефиниран по описания тук: Настройки на системния регистър [на IRM за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ако все още имате проблеми, съберете регистрационни файлове на клиента за защита на информацията в Azure и прикачете експортираните регистрационни файлове към този билет.

1. Отворете документ на Office или създайте нов имейл в Outlook.
2. Щракнете **върху Помощ за защита/чувствителност** и обратна  >  **връзка.**
3. Щракнете **върху Експортиране на регистрационни файлове**.
4. Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към тази заявка за услуга.

Допълнителни ресурси:

- [Как да конфигурирате етикет за визуални маркировки за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Използване на етикети за чувствителност в приложения на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

