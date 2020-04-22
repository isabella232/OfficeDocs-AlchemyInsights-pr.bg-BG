---
title: 2681 атака симулатор в Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 74bd2dd62b24aaf6c9d7b387ab1d97ddab31e902
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713455"
---
# <a name="attack-simulator-in-microsoft-365"></a>Симулатор на атаки в Microsoft 365

- Липсва ли симулатор на атака? Симулатор ът на атаки изисква **План за разширена защита на заплахите 2 на Office (ATP план 2)** или **Office 365 Enterprise E5**. Симулатор на атаки **не** е включен в План за защита от заплахи на Office 365 1 (ATP план 1), Office 365 Enterprise E3 или всички приложения на Microsoft 365 за бизнес абонаменти.

- Акаунтът, който използвате за стартиране на симулирани атаки изисква разрешения на глобален администратор или администратор на защитата и многофакторно удостоверяване (МВНР). За повече информация относно изискванията за симулатор на атака вижте [тази тема](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Важни неща, които трябва да знаете за симулации на атака **Brute Force Password:**

  - Ако целевият акаунт е активирана и паролата е отгатната правилно, акаунтът няма да се показва като компрометирана (вторият фактор за удостоверяване ще бъде непълен).

  - Файлът с парола не може да бъде по-голям от 10 МБ. Използвайте по една парола на ред и включете празен ред (връщане на каретата) след последната парола в списъка.

- Важни неща, които трябва да знаете за фишинг симулациите **на Spear Phishing:**

  - По дизайн не можете да предоставите потребителска стойност за URL адрес на сървър за **влизане в фишинг**.

  - Ако получателят използва [добавката Разрешаване на съобщението](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) за съобщаване за съобщение като фишинг, може да не получавате предупреждения за съобщението (защото това е симулирана атака).

- Отчети: След като симулирана атака завърши, можете да щракнете върху **Подробности за атаката,** за да видите отчета.

- За подробни инструкции и нови функции в атака [симулатор, вижте Атака симулатор в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
