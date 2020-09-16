---
title: Симулатор за атаки на 2681 в Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759208"
---
# <a name="attack-simulator-in-microsoft-365"></a>Симулатор за атаки в Microsoft 365

- Липсващ симулатор за атаки ли сте? Симулаторът за атаки изисква **office 365 Advanced Protection Plan 2 (ATP план 2)** или **Office 365 Enterprise E5**. Симулаторът за атаки **не** е включен в Office 365 Advanced план за защита от заплахи 1 (ATP план 1), Office 365 Enterprise E3 или Microsoft 365 приложения за бизнес абонаменти.

- Акаунтът, който използвате, за да стартирате симулираните атаки, изисква глобален администратор или разрешения на администратора на защитата и многофакторно удостоверяване (МВНР). За повече информация относно изискванията за симулатор на атаки вижте [тази тема](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Важни неща, които трябва да знаете за симулационните симулации за атаки с **парола на груба сила**

  - Ако целевият акаунт има активиран и паролата е отгатната правилно, акаунтът няма да се показва като компрометиран (Вторият фактор за удостоверяване ще бъде непълен).

  - Файлът с парола не може да е по-голям от 10 МБ. Използвайте една парола на ред и включвайте празен ред (връщане на превоз) след последната парола в списъка.

- Важни неща, които трябва да знаете за **копието на фишинг** прикачване на симулации:

  - По проект не можете да предоставите стойност по избор за **URL адрес на фишинг сървъра за влизане**.

  - Ако получател използва [добавката разрешаване на съобщение за отчет](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , за да съобщи съобщението като фишинг, е възможно да не получавате предупреждения за съобщението (защото това е симулация на атака).

- Отчети: след като симулираната атака завърши, можете да щракнете върху **подробности за атака** , за да видите отчета.

- За подробни инструкции и нови функции в симулатора за атаки вижте [симулатор за атаки в Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
