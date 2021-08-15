---
title: Грешки при синхронизиране на автоматично записване на устройства на Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013737"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Грешки при синхронизиране на автоматично записване на устройства на Apple

"Открихме, че имате един или повече ADE/DEP маркери, които са в състояние на грешка. Докато състоянието на грешката не бъде коригирано за всеки засегнат маркер, функционалността ADE няма да работи според очакванията.".

Тази грешка може да се прояви по редица начини, включително:

1. Възможно е устройствата да не се синхронизират от ABM/ASM с Intune
2. Назначения на профил за записване може да са неуспешен
3. Възможно е устройствата да не завършат успешно записването за ADE

Проверете за грешката при синхронизиране, съобщена в конзолата Intune под Устройства > Записване на устройства > записване на Apple > Маркери **на програмата Записване.**

Една от най-често срещаните причини за грешка при синхронизиране е изтичането на текущия маркер. В много случаи подновяването на засегнатия маркер ще реши проблема.

Ако един или повече от вашите маркери са изтекли, вижте следната документация, за да ви помогне да ги подновите, както е подходящо:

[Подновяване на маркер за записване на автоматизирано устройство](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Освен това можете да видите следната документация, за да видите възможните коригирания за други грешки, които причиняват грешки при синхронизиране на маркери:

[Грешки при синхронизиране на ABM/ASM за маркери за записване на устройства за iOS/iPadOS и macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Грешки при синхронизиране на ABM/ASM за маркери за записване на устройства за iOS/iPadOS и macOS](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
