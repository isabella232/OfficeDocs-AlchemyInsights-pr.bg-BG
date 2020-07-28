---
title: Промяна на каналите за актуализиране на приложенията на Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438762"
---
# <a name="change-update-channels-for-office-apps"></a>Промяна на каналите за актуализиране на приложенията на Office

За нови инсталации на Office използвайте настройките за изтегляне на софтуер от Office, за да изберете желания канал за актуализация, след което инсталирайте (или инсталирайте отново) приложения на Office. За повече информация вижте [Управление на настройките за изтегляне на софтуер в Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Забележка:** Канал за актуализация, избран с помощта на настройките за изтегляне на софтуер от Office се отнася за всички потребители, които изпълняват нови инсталации с помощта на портала O365. За повече информация вижте [Изтегляне и инсталиране или преинсталиране на Microsoft 365 или Office 2019 на компютър pc или Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

За съществуващите инсталации на Office използвайте инструмента за разполагане на Office (ODT) да преминете към друг канал за актуализация:  

1. Изтеглете последната версия на инструмента за разполагане на Office (setup.exe) от центъра на [Microsoft за изтегляния](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Определете името на канала, към който искате да превключите. За повече информация вижте [Опции за конфигуриране на инструмента за разполагане на Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Създаване на конфигурация XML файл, указващ името на канала, например update.xml.  
    A. <Configuration>  
    B. <актуализации **канал= "месечно"** />  
    C. </Configuration>
4. От команден ред с повишени потребителски права преминете към папката, където setup.exe се намира и изпълнете следната команда:  
    A. setup.exe /конфигуриране update.xml
5. Стартирайте приложение от Office (например Excel) и след това изберете **Акаунт на файл**  >  **Account**. В секцията Информация за продукта изберете **Актуализиране на опциите**  >  **актуализирай сега**.

За повече информация вижте [Как да превключвате актуализиране на канали за съществуващи приложения на Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

За превключване актуализиране канали за избрана група от потребители или чрез Configuration Manager (SCCM) конфигурирайте настройката за актуализиране на канал с помощта на GPO. За повече информация вижте [Преглед на каналите за актуализация за приложения на Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). За подробности вижте [Как да управлявате Office 365 ProPlus Канали за ИТ професионалисти](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) и управление на актуализации на Приложения на Microsoft [365 с Диспечер на конфигурационните настройки на Microsoft endpoint.](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager)