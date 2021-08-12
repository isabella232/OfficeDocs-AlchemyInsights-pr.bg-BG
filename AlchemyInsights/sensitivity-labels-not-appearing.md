---
title: Етикетите за чувствителност не се показват
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061421"
---
# <a name="sensitivity-labels-not-appearing"></a>Етикетите за чувствителност не се показват

Етикетите за чувствителност ви позволяват да класифицирате и да помогнете за защитата на вашето чувствително съдържание. Те могат да бъдат създадени в центъра за Център за съответствие на Microsoft 365, Microsoft 365 защита или центъра за Microsoft 365 защита & съответствие под Етикети за класификация > Чувствителност. За да научите повече за тази функция, вижте [Общ преглед на етикетите за чувствителност](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ако сте конфигурирали етикетите за чувствителност, но те не се показват в Microsoft 365 приложения, проверете следното:

- Уверете се, че етикетът за чувствителност [е публикуван](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) за потребителите и групите, които искате.

- Уверете се, че потребителят използва приложение, което поддържа етикети за чувствителност – вижте [етикетите за чувствителност във вашия документ.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- Ако мигрирате [етикети за защита на информацията в Azure,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)имайте предвид съображенията, изброени [тук.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Поддръжка за защита от загуба на данни (DLP): В момента само етикетите за съхранение могат да се използват като условие в правилата за DLP.  Поддръжката за етикети за чувствителност в DLP правила все още не е налична, но работим по нея.

- Когато шифроването е разрешено на етикет за чувствителност, можете да изберете едно от двете:
    - Дайте разрешения сега
    - Позволяване на потребителите да присвояват разрешения


За повече информация относно възможните проблеми вижте [Известни проблеми с етикетите за чувствителност](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).