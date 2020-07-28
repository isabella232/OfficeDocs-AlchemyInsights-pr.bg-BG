---
title: Управление на автоматичните актуализации за приложенията на Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438754"
---
# <a name="control-automatic-updates-for-office-apps"></a>Управление на автоматичните актуализации за приложенията на Office

По подразбиране актуализациите за приложенията на Office се изтеглят автоматично и се прилагат във фонов режим без намеса на потребителя. Обаче администраторите могат да контролират как актуализациите се прилагат с помощта на настройките за актуализиране на Office. Актуализиране на настройките позволяват на администраторите да разрешават или забраняват автоматичните актуализации, да показват или скриват бутона **"Актуализирай сега"** в Office, да зададете срокове за актуализиране и други. За подробна информация вижте:

- [Конфигуриране на настройките за актуализация за Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Не е разрешено автоматично актуализиране на Office](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Определяне на начина на актуализиране на Office след инсталирането му](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

За да прегледате съществуващите настройки за актуализации, приложени към клиентски компютър, изпълнете следните стъпки:

1. Отворете редактора на системния регистър, като **отидете да**  >  **стартирате**  >  **regedit**.
2. Превключете на следното местоположение и прегледайте настройките за актуализиране на Office:  
    A. HKEY_LOCAL_MACHINE\СОФТУЕР\Microsoft\Office\  
    B. Щракнете върху "Изпълнение\Конфигуриране"

**Забележка:**  Ако ключът OfficeMgmtCOM е зададен, може да видите "Актуализации се **Office**управляват от вашия системен администратор" съобщение в  >  **Office акаунт**Office  >  **актуализации**. За повече информация вижте [Управление на актуализации на Приложения на Microsoft 365 с Диспечер на конфигурационните данни на Microsoft за крайна точка](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  