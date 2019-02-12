---
title: Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: aa2262ed487ae4160f13490e92163a145e657862
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934765"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Отстраняване на проблеми с регистрирате Windows устройства в Microsoft Intune

Преглед на ресурси, изброени по-долу да решим вашия проблем сега. 
  
Някои често срещани съобщения за грешка и разрешаване стъпки:
  
 **Не може да бъде инсталиран софтуер, 0x80cf4017:** Сертификат вашия акаунт е изтекъл. Повторно изтегляне компютър клиент софтуерен пакет в на Intune административната конзола. Прегледайте документацията за повече информация. 
  
 **Код на грешка 0x801c0003:** Тази грешка може да възникне в следните сценарии: 
  
1. Потребителят има повече устройства, записани от лимита за устройството. Преглед на тези документи, за да [премахнете устройството](https://docs.microsoft.com/intune/devices-wipe) или [променете лимита за устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Потребителите може да присъедини устройства към лазурните АД" е настроен на "няма". Поставям то към всички или изберете потребители. Прегледайте [документацията](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация. 
    
3. Устройството вече е записан от друг потребител. Ако случаят е такъв, премахнете устройството от Azure Intune конзола или ръчно unenroll устройство преди да опитате отново.
    
4. Устройството е Windows 10 Начало. Само Windows 10 Pro, образование и предприятието ие може да обединяват Azure Active Directory.
    
Допълнителни ресурси за разрешаване на вашия проблем:
  
1. Използвате [Intune портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на общи записване неизправности. Преглед на [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности. 
    
2. Преглед на тези документи за списък на често срещани грешки, които пречат на записване и резолюции на всеки: [ръководство за отстраняване на проблеми](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [отстраняване на док](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Научете как да се запишат устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

