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
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934282"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Правилата не се държат според очакванията

Защита на информацията в Azure: Правилата не се държат според очакванията, вижте следното за препоръчителни указания за различни проблеми с правилата:

1. Ако имате проблеми с визуалните маркировки, прегледайте [При прилагане на визуални маркировки.](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)
2. Ако имате проблеми с автоматичното етикетиране, прегледайте Как да конфигурирате условията за автоматична и препоръчителна класификация за защита на информацията в [Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и Какво търси типовете [поверителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ако имате проблеми със защитата native/Pfile, прегледайте конфигурирането [на API на файл](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Проверете дали използвате правила с обхват, които не са конфигурирани правилно: Как да конфигурирате правилата за защита на информацията в Azure за определени потребители с [помощта на правилата с обхват.](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)
5. Ако автоматичното етикетиране не работи за Outlook при прикачване на етикетиран документ, проверете дали DRMEncryptProperty не е дефиниран по описания тук: [настройки на IRM системния регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ако все още имате проблеми, съберете регистрационни файлове на клиента за защита на информацията в Azure и прикачете експортираните регистрационни файлове към този билет.

1. Отворете документ Office или създайте нов имейл в Outlook.
2. Щракнете **върху Помощ за защита/чувствителност** и обратна  >  **връзка.**
3. Щракнете **върху Експортиране на регистрационни файлове**.
4. Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към тази заявка за услуга.

Допълнителни ресурси:

- [Как да конфигурирате етикет за визуални маркировки за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Използване на етикети за чувствителност Microsoft 365 приложения](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

