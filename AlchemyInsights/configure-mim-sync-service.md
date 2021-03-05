---
title: Конфигуриране на услугата за синхронизиране на мим
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480900"
---
# <a name="configure-mim-sync-service"></a>Конфигуриране на услугата за синхронизиране на мим

Услугата за синхронизация на Microsoft Identity Manager (мим) е компонент на мим. Това е централизирана локална услуга, която съхранява и интегрира информация за организации, които имат множество локални указатели и бази данни. Възможно е да успеете да отстраните проблема си с мим Sync, ако проблемът е адресиран в скорошна актуализация за мим или е един от другите проблеми, упоменати в раздела по-долу.

**Препоръчителни стъпки**

1. Уверете се, че използвате скорошна актуализация на мим Sync и проверете [бележките за изданието на мим за синхронизиране](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , за да определите дали проблемът е разрешен в актуализация.
2. Ако проблемът е с генеричните LDAP, Generic SQL, Lotus Domino или Web Services Connector, уверете се, че използвате скорошна актуализация на [генеричните конектори](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).
3. Ако даден мим за синхронизиране спре с грешка, прегледайте таблицата с кодове на [грешки при изпълнение](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , за да определите потенциалните причини.
4. Ако изпълнението спира с **разширение-DLL-изключение**, след това щракнете върху тези думи, за да отворите прозореца **за свойства на обекта на конектора** , след което щракнете върху **проследяване на стека...** , за да видите повече информация за основната причина, както е описано в [разширение-DLL-изключение](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).
5. Ако функцията за известяване при промяна на парола (PCNS) съобщава за **грешка 6025** в регистъра на събитията по време на синхронизирането на пароли, прегледайте справочника за отстраняване на неизправности при [Съобщаване за грешки в PCNS на 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).
6. Ако пълната синхронизация с агента за управление на FIM услугата е бавна, Проверете настройката за **автоматично нарастване** за TempDB, както е описано в [отстраняване на неизправности или висящо пълно синхронизиране](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).
7. Ако се сблъскате с грешка от спряно сървъра с Неуспешно създаване на уеб-услуги с помощта на агента за управление на FIM услуга, вижте [поддръжка-info: Неуспешно създаване-уеб-услуги](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) за общ преглед на причините.

