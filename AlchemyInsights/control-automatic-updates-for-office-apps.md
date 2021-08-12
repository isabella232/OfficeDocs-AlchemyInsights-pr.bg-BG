---
title: Управление на автоматичните актуализации за Office приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: f162f11f678e8673d85e52cd9e54cedd7bd6e6a3aee87fcb2731a06d2698ea6a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929870"
---
# <a name="control-automatic-updates-for-office-apps"></a>Управление на автоматичните актуализации за Office приложения

По подразбиране актуализациите за Office се изтеглят автоматично и се прилагат във фонов режим без намеса на потребителя. Администраторите обаче могат да контролират как се прилагат актуализациите с помощта на Office за актуализиране. Настройките за актуализиране позволяват на администраторите да разрешават  или забраняват автоматични актуализации, да показват или скриват бутона Актуализирай сега в Office, да задават крайни срокове за актуализиране и др. За подробна информация вижте:

- [Конфигуриране на настройките за актуализиране за Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Автоматичното актуализиране за Office не е разрешено](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Дефиниране на Office се актуализира, след като е инсталиран](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

За да прегледате съществуващите настройки за актуализации, приложени към клиентския компютър, изпълнете следните стъпки:

1. Отворете редактора на системния регистър, като отворите **"Старт**  >    >  **изпълнение" regedit**.
2. Превключете на следното местоположение и прегледайте Office "Актуализиране":  
    a. HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Забележка**  Ако е зададен клавишът OfficeMgmtCOM, може да видите съобщението "Актуализациите се управляват от вашия системен **администратор" в Office**  >  **акаунт**  >  **Office Актуализации**. За повече информация вижте Управление [на актуализациите за Приложения на Microsoft 365 с Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  