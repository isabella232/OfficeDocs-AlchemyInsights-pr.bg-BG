---
title: Не е възможно влизане в Teams поради грешка autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 6671a63d97f24fadc9b34907d75600a3c0ad1c9990a4a8f8d32034c11e8a952e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038389"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Не е възможно влизане в Teams поради грешка autologon.microsoftazuread-sso точка com:443

Ако Seamless SSO е разрешено като удостоверяване на O365, може да е необходимо URL адресът autologon.microsoftazuread-sso.com да се добави към "Интранет сайтове".  Ако той вече е добавен към "Надеждни сайтове", при използване на Seamless SSO той трябва да бъде премахнат от "Надеждни сайтове".

Прегледайте [контролен списък за отстраняване на неизправности със Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Изпълнете следните стъпки, за да добавите URL адрес към списъка "Интранет сайтове":

1. Отворете Internet Explorer, като щракнете върху бутона **Старт**. В полето за търсене въведете Internet Explorer и след това в списъка с резултати щракнете върху **Internet Explorer**.
2. Щракнете върху **Инструменти** и след това – върху **Опции за интернет**.
3. Щракнете върху раздела **Защита**.
4. Сега щракнете върху **Локални интранет сайтове**, а след това щракнете върху бутона **Сайтове** и след това върху бутона **Разширени**.
5. Въведете URL адреса на уеб сайта и щракнете върху **Добави**.
6. Когато приключите, щракнете върху **Затвори**.

За повече информация вж. [Документация за разполагане на Seamless SSO за O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (включва базиран на правила процес за добавяне на URL адрес към интранет сайтове в стъпка 3).
