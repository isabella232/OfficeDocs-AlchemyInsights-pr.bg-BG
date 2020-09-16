---
title: 'ПДИ: правилата не се оказват по очаквания начин'
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
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663178"
---
# <a name="aip-policies-not-behaving-as-expected"></a>ПДИ: правилата не се оказват по очаквания начин

Защита на информацията за Azure: правилата не се очакват по очаквания начин, вижте следните Препоръчителни указания за различни проблеми с правилата:

1. Ако имате проблеми с визуалните маркировки, моля, прегледайте [Кога се прилагат визуални маркировки](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Ако имате проблеми с автоматичното етикетиране, прегледайте [как да конфигурирате условия за автоматична и Препоръчителна класификация за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) и [за какво се търсят типовете чувствителна информация](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Ако имате проблеми с Native/Pfile Protection, моля, прегледайте [конфигурацията на API на файла](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Проверете дали използвате правила за обхват, които не са конфигурирани правилно: [как да конфигурирате Azure Policy Protection за определени потребители, като използвате правила за обхват](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Ако автоматичното етикетиране не работи за Outlook при прикачването на документ с етикети, уверете се, че DRMEncryptProperty не е дефиниран, както е описано тук: [Настройки за IRM регистър за защита](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Ако все още имате проблеми, моля, съберете регистрите на клиентите на Azure за защита на информацията и прикачете експортираните регистрационни файлове към този билет.

1. Отворете документ на Office или създайте ново имейл съобщение в Outlook.
2. Щракнете **Protect/Sensitivity**върху  >  **помощ и обратна връзка**за защита/чувствителност.
3. Щракнете върху **експортиране на регистрационни файлове**.
4. Запишете регистрите по ваш избор на местоположение и ги прикачете към това искане за обслужване.

Допълнителни ресурси:

- [Как да конфигурирате етикет за визуалните маркировки за Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Преглед на документацията за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Използване на етикети за чувствителност в приложенията на Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

