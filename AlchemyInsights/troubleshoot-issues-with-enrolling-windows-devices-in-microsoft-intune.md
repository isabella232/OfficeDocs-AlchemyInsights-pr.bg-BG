---
title: Отстраняване на проблеми при записването на устройства с Windows в Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658867"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Отстраняване на проблеми при записването на устройства с Windows в Microsoft

Прегледайте ресурсите, изброени по-долу, за да решите проблема си сега.
  
Някои често срещани съобщения за грешка и стъпки за разрешаване:
  
 **Софтуерът не може да се инсталира, 0x80cf4017:** Вашият сертификат за акаунт е изтекъл. Изтеглете отново пакета за софтуерни клиенти на PC в конзолата за администриране на администратора. Прегледайте тази документация за повече информация.
  
 **Код на грешка 0x801c0003:** Грешката може да възникне в следните сценарии:
  
-  Потребителят има повече устройства, записани от лимита на устройството. Прегледайте тези документи, за да [премахнете устройство](https://docs.microsoft.com/intune/devices-wipe) или да [промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Потребителите могат да се присъединят към устройства в Azure AD" е зададено на "няма". Настройте го на всички или изберете потребители. Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.

-  Устройството вече е записано от друг потребител. Ако това е така, премахнете устройството от конзолата за настройване на Azure или ръчно отменете устройството, преди да опитате отново.

-  Устройството е Windows 10 Home. Само Windows 10 Pro, Education и Enterprise МСА могат да се присъединят към Azure Active Directory.

Допълнителни ресурси, които да ви помогнат да отстраните проблема:
  
-  Използвайте [портала за отстраняване на неизправности](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , за да диагностицирате и отстраните чести неуспешни записвания. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

-  Прегледайте тези документи за списък с често срещани грешки, които пречат на записването и резолюциите във всеки от тях: [ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и [отстраняване на неизправности](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Научете как да записвате устройства с Windows в Microsoft](https://docs.microsoft.com/intune/windows-enroll).
