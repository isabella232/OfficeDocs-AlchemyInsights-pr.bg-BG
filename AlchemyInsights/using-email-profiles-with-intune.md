---
title: Използване на имейл профили с Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919412"
---
# <a name="using-email-profiles-with-intune"></a>Използване на имейл профили с Intune

Intune може да се използва за създаване и разполагане на имейл профили за основен (вграден) имейл клиент на множество платформи на устройства.

За информация относно някои от ограниченията, свързани с имейл профилите, включително как се обработват наличието на съществуващи профили и как да премахнете имейл профили, вижте Добавяне на настройки за имейл към устройства [с помощта на Intune](https://docs.microsoft.com/intune/email-settings-configure).

За повече информация как да създадете имейл профили за всяка платформа на устройство, вижте:

[Настройки на устройството с Android за конфигуриране на имейл, удостоверяване и синхронизиране в Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Добавяне на настройки за имейл за устройства с iOS и iPadOS в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Настройки на имейл профил в Microsoft Intune за устройства с Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Настройки на имейл профил за устройства, изпълняващи Windows 10 в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Често срещан проблем при синхронизиране**

**ИМЕЙЛ профилът на KNOX в Android не позволява на потребителите контакти, календар и задачи да се синхронизират с потребителски устройства.**

KNOX в имейл профила на Android KNOX предлага на администратора опцията да реши кои типове съдържание да се синхронизират с устройството, като зададете всеки от тях да бъде разрешен.

Ако настройката за някой от типовете съдържание е зададена на **Не** е конфигурирана (по подразбиране), този тип съдържание не се синхронизира автоматично. Потребителят може да разреши типа съдържание, който иска, директно на устройството ръчно, но тази конфигурация се замества от настройката на правилата на Intune, а синхронизирането спира за този тип съдържание.

