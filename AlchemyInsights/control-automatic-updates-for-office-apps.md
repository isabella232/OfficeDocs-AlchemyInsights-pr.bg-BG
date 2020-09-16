---
title: Управление на автоматични актуализации за приложенията на Office
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
ms.openlocfilehash: ab3d6e60bc1b67220adbdf7ba61599a6b7aa663a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747765"
---
# <a name="control-automatic-updates-for-office-apps"></a>Управление на автоматични актуализации за приложенията на Office

По подразбиране актуализациите за приложенията на Office се изтеглят автоматично и се прилагат във фона без намесата на потребителя. Администраторите обаче могат да управляват как се прилагат актуализациите с помощта на настройките на Office Update. Настройки за актуализиране Позволяване на администраторите да разрешават или забраняват автоматични актуализации, да показват или скриват бутона **Актуализирай сега** в Office, да задават срокове за актуализиране и др. За по-подробна информация вижте:

- [Конфигуриране на настройките за актуализиране за Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Автоматичното актуализиране за Office не е разрешено](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Определяне как Office да се актуализира, след като е инсталиран](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

За да прегледате съществуващите настройки за актуализации, приложени към клиентска машина, изпълнете следните стъпки:

1. Отворете редактора на системния регистър, като отидете на **Старт**  >  **Run**  >  **regedit**.
2. Преминете към следното местоположение и Прегледайте настройките за актуализиране на Office:  
    на. HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft\Office\  
    b. ClickToRun\Configuration

**Забележка**  Ако клавишът OfficeMgmtCOM е зададен, може да видите съобщение "актуализациите се управляват от вашия системен администратор **" в**актуализации на Office  >  **акаунт**за Office  >  **Office Updates**. За повече информация вижте [управление на актуализациите за приложенията на microsoft 365 чрез диспечера за конфигуриране на крайна точка на Microsoft](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  