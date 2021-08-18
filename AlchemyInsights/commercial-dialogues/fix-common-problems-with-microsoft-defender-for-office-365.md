---
title: Коригиране на често срещани проблеми с Microsoft Defender за Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330049"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Коригиране на често срещани проблеми с Microsoft Defender за Office 365

Ето някои решения на често срещани проблеми с Microsoft Defender за Office 365:

- **Забавяне на съобщението:**

  Закъсненията в доставянето на имейли може да са причина за Сейф на прикачени файлове, сканиращи съобщения. За повече информация вж. [Сейф на правилата за прикачени файлове](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Отчет за грешни положителни или отрицателни резултати:**

  За повече информация вижте Докладване [на съобщения и файлове на Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft).

- **Разрешаване Сейф на връзката:**

  1. В портала Microsoft 365 Defender отидете на Имейл & за сътрудничество & правила за <https://security.microsoft.com/>  \>  \>  \> **заплахи Сейф връзки** в **раздела** Правила.

     За да отидете директно на **страницата Сейф връзки,** използвайте <https://security.microsoft.com/safelinksv2> .

  2. На страницата **Сейф връзки** изберете правилата, като щракнете върху името на правилата.
  3. В допълнителната информация, която се появява, направете някоя от следните стъпки:
     - За да добавите нови правила, изберете **+ Създаване**. Съветникът ще се стартира, за да ви помогне да дефинирате настройките на правилата си.
     - За да редактирате съществуващи правила, изберете правилата, като щракнете върху името на правилата. В менюто с подробни данни, което се появява, **изберете Редактиране** в **секцията Настройки на** защитата.
  4. На страницата **Настройки за** защита конфигурирайте следните настройки:
     - Включете Изберете **действието за неизвестни потенциално злонамерени URL адреси в съобщенията.**
     - Изберете **Прилагане на безопасни връзки към съобщения, изпратени в организацията.**

  За повече информация вижте [Настройване на правила Сейф връзки в Microsoft Defender за Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
