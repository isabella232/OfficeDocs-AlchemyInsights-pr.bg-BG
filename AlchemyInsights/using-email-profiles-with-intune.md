---
title: Използване на имейл профили с Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554743"
---
# <a name="using-email-profiles-with-intune"></a>Използване на имейл профили с Intune

Intune може да се използва за създаване и внедряване на имейл профили за основен (вграден) имейл клиент на няколко платформи на устройства.

За информация относно някои от ограниченията, свързани с имейл профили, включително как се обработват съществуващите профили и как се премахват имейл профилите, вижте [Добавяне на настройки за имейл към устройства, използващи Intune](https://docs.microsoft.com/intune/email-settings-configure).

За повече информация относно създаването на имейл профили за всяка платформа на устройството вижте:

[Настройки на устройството с Android за конфигуриране на имейл, удостоверяване и синхронизиране в Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Добавяне на настройки за електронна поща за iOS и iPadOS устройства в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Настройки на имейл профил в Microsoft Intune за устройства с Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Настройки на имейл профила за устройства с Windows 10 в Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Често срещан проблем при синхронизиране**

**KNOX в имейл профила на Android не позволява на потребителски контакти, календар и задачи, синхронизиране на потребителски устройства.**

В KNOX на Android KNOX имейл профил предлага на администратора възможност да реши кои типове съдържание са синхронизирани на устройството чрез настройка всеки да е активиран.

Ако настройката за някой от типовете съдържание е зададена на **Не е конфигуриран** (по подразбиране), този тип съдържание не е синхронизиран автоматично. Потребителят може да разреши типа на съдържанието, който иска ръчно директно на устройството, но тази конфигурация се замества от настройката на правилата на Intune и синхронизирането спира за този тип съдържание.

