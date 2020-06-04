---
title: Отстраняване на проблеми със записване на устройства с Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665821"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Отстраняване на проблеми със записване на устройства с Windows в Microsoft Intune

Прегледайте ресурсите, изброени по-долу, за да разрешите проблема си сега.
  
Някои често срещани съобщения за грешки и стъпки за разрешаване на проблема:
  
 **Софтуерът не може да бъде инсталиран, 0x80cf4017:** Вашият сертификат за акаунт е изтекъл. Изтеглете отново клиентския пакет за PC в Intune Admin Console. Прегледайте тази документация за повече информация.
  
 **Код на грешка 0x801c0003:** Грешка може да възникне в следните ситуации:
  
-  Потребителят има повече включени устройства от ограничението на устройството. Прегледайте тези [документи, за](https://docs.microsoft.com/intune/devices-wipe) да премахнете устройство или [да промените ограничението на устройството](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Потребителите могат да се присъедини устройства Azure AD" е зададена на "няма". Задайте го на всички или изберете потребители. Прегледайте [тази документация](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) за повече информация.

-  Устройството вече е записано от друг потребител. Ако случаят е такъв, премахнете устройството от Azure Intune конзолата или ръчно откройте устройството, преди да опитате отново.

-  Устройството е Windows 10 Home. Само Windows 10 Pro, образование и корпоративните skus могат да се присъединят към Azure Active Directory.

Допълнителни ресурси за разрешаване на проблема:
  
-  Използвайте [Intune Отстраняване на неизправности портал](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) за диагностика и разрешаване на често срещани записване грешки. Прегледайте [този документ](https://docs.microsoft.com/intune/help-desk-operators) за повече подробности.

-  Прегледайте тези документи за списък с често срещани грешки, които пречат на записване и решения за всеки от тях: [Ръководство за отстраняване на неизправности](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) и отстраняване на неизправности [.](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)

[Научете как да записвате устройства с Windows в Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
