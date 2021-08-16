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
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065273"
---
# <a name="attack-simulator-in-microsoft-365"></a>Атака на тренажор в Microsoft 365

- Липсва ли ви таен тренажор? Симулаторът на атаки **изисква Microsoft Defender Office 365 план 2** или Office 365 Enterprise **E5**. Симулаторът на **атаки не** е включен в Microsoft Defender за Office 365 план 1, Office 365 Enterprise E3 или Приложения на Microsoft 365 за бизнеса абонаменти.

- Акаунтът, който използвате за стартиране на симулирани атаки, изисква разрешения на глобален администратор или администратор на защитата и многофакторно удостоверяване (MFA). За повече информация относно изискванията за таен тренажор [за атаки вж. тази тема.](/microsoft-365/security/office-365-security/attack-simulator)

- Важни неща, които трябва да знаете за **симулации за атака с** парола на Brute Force:

  - Ако целевият акаунт е разрешен за MFA и паролата е била познана правилно, акаунтът няма да се покаже като компрометиран (вторият фактор за удостоверяване ще бъде непълен).

  - Файлът с парола не може да бъде по-голям от 10 МБ. Използвайте по една парола на ред и включете празен ред (връщане на каретата) след последната парола в списъка.

- Важни неща, които трябва да знаете за **прикачването на симулации** за фишинг на Spear:

  - По проект не можете да предоставите стойност по избор за URL адрес на сървъра за **фишинг влизане.**

  - Ако получателят използва добавката [Разреши](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) съобщението за отчет, за да съобщи за съобщението като фишинг, е възможно да не получавате известия за съобщението (тъй като това е симулирана атака).

- Отчети: След като симулираната атака завърши, можете да щракнете върху Подробни данни **за атаката,** за да видите отчета.

- За подробни инструкции и нови функции в симулатора на атаки вижте [Симулатор на атаки в Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)
