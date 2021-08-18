---
title: 2681 Attack Simulator в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325060"
---
# <a name="attack-simulator-in-microsoft-365"></a>Атака на тренажор в Microsoft 365

- Липсва ли ви таен тренажор? Симулаторът на **атаки изисква Microsoft Defender Office 365 план 2** или Office 365 Enterprise **E5**. Симулаторът на **атаки не** е включен в Microsoft Defender за Office 365 план 1, Office 365 Enterprise E3 или Приложения на Microsoft 365 за бизнеса абонаменти.

- Акаунтът, който използвате за стартиране на симулирани атаки, изисква разрешения на глобален администратор или администратор на защитата и многофакторно удостоверяване (MFA). За повече информация относно изискванията за таен тренажор [за атаки вж. тази тема.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Важни неща, които трябва да знаете за **симулации за атака с** парола на Brute Force:

  - Ако целевият акаунт е разрешен за MFA и паролата е била познана правилно, акаунтът няма да се показва като компрометиран (вторият фактор за удостоверяване ще бъде непълен).

  - Файлът с парола не може да бъде по-голям от 10 МБ. Използвайте по една парола на ред и включете празен ред (връщане на карета) след последната парола в списъка.

- Важни неща, които трябва да знаете за **прикачването на симулации** за фишинг на Spear:

  - По проект не можете да предоставите стойност по избор за URL адрес на сървъра за **фишинг влизане.**

  - Ако получателят използва добавката [Разреши](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) съобщението за отчет, за да съобщи за съобщението като фишинг, е възможно да не получавате известия за съобщението (тъй като това е симулирана атака).

- Отчети: След като симулираната атака завърши, можете да щракнете върху Подробни данни **за атаката,** за да видите отчета.

- За подробни инструкции и нови функции в симулатора на атаки вижте [Симулатор на атаки в Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
