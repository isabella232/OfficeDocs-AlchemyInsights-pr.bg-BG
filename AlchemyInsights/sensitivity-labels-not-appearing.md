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
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801173"
---
# <a name="sensitivity-labels-not-appearing"></a>Етикетите за чувствителност не се показват

Етикетите за чувствителност ви позволяват да класифицирате и да защитавате чувствителното съдържание. Те могат да бъдат създадени в центъра за съответствие на Microsoft 365, в центъра за защита на Microsoft 365 или в центъра за защита на & на Microsoft 365 под класификация > етикети за чувствителност. За да научите повече за тази функция, вижте [общ преглед на етикетите за чувствителност](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Ако сте конфигурирали вашите етикети за чувствителност, но те не се показват в приложенията на Microsoft 365, проверете следното:

- Уверете се, че етикетът за чувствителност е [публикуван](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) за потребителите и групите, които искате.

- Уверете се, че потребителят използва приложение, което поддържа етикети за чувствителност – вижте [етикети за чувствителност във вашия документ](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Ако [мигрирате етикети на Azure за защита на информацията](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), имайте предвид съображенията, описани [тук](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).

- Поддръжка за предотвратяване на загуба на данни (DLP): в момента само етикети за съхранение могат да бъдат използвани като условие в DLP правила.  Поддръжката за етикети за чувствителност в DLP правилата все още не е налична, но работим по него.

- Когато шифроването е разрешено на етикет за чувствителност, можете да изберете:
    - Присвояване на разрешения сега
    - Позволяване на потребители да присвояват разрешения


За повече информация относно възможните проблеми вижте [известни проблеми с етикети за чувствителност](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).