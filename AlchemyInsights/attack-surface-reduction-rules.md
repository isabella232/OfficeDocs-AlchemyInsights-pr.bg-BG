---
title: Правила за намаляване на повърхността на атака
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676072"
---
# <a name="attack-surface-reduction-rules"></a>Правила за намаляване на повърхността на атака

Изключването на файлове или папки може сериозно да намали защитата, предоставена от правилата за намаляване на повърхността на атаката. Файловете, които биха били блокирани от правило, могат да се изпълняват и не се записва отчет или събитие. Изключение се отнася за всички правила, които позволяват изключения.

Изключенията от ASR използват същия синтаксис като Microsoft Defender Antivirus изключения. За подробности вижте Конфигуриране [и проверка на изключения за Microsoft Defender Antivirus сканирания](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus). За да избегнете проблеми, [прегледайте Често срещани грешки, за да избегнете при дефиниране на изключения](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).

Не всички правила за ASR поддържат изключения. За да проверите дали вашето правило поддържа изключения, вижте таблицата Правила за намаляване [на повърхността на атака](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Правила за намаляване на повърхността на атака

Повърхността на атаката на вашата организация включва всички места, където хакер може да компрометира организационни устройства или мрежи. Намаляването на повърхността на атаката означава защита на организационните устройства и мрежата, което оставя на хакерите по-малко начини за извършване на атаки. Конфигурирането на правилата за намаляване на повърхността на атаката в Microsoft Defender за крайна точка може да ви помогне.

За повече информация вижте:

- [Map ASR правило GUID за име](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- Изисквания към правилата за ASR:
    - [Windows 10 Pro, версия 1709 или по-нова](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, версия 1709 или по-нова](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Сървър, версия 1803 (полугодишен канал) или по-нова версия](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Идентифициране на правилното изключване, което да се приложи

1. Потърсете eventID 1121 или 1122 в регистрационния файл на Microsoft-Windows-Windows Defender/Операционен.

1. Оценете сценария и контекста на блока и потвърдете, че този сценарий трябва да бъде разблокиран.

1. Прочетете стойността Път в подробните данни за събитието, което е стойността, която дефинира изключението.
    - Направете изключението възможно най-строго.
    - Прилагане на заместващ символ, когато е необходимо (например заместване на променливата потребител).

1. Приложете изключението според нуждите ви от разполагане. За подробности вижте Персонализиране на [правилата за намаляване на повърхността на атаката](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).

## <a name="exclusion-is-not-honored"></a>Изключването не е зачетено

1. Определете дали правилото поддържа изключения. За подробности вижте Правила за [намаляване на повърхността на атака](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Прегледайте приложените изключения и проверете с данните за събитието за правописни грешки или неправилно интерпретирани заместващи символи. За повече информация вижте [Поддържани типове изключения](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ако въздействието на правилото е твърде високо, помислете за преместване на правилото (обратно) в режим на проверка, за да извършите по-нататъшно валидиране. За подробности вижте Тестване как [функциите на Microsoft Defender за крайна точка работят в режим на проверка.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Събирайте данни за поддръжка, за да отворите случай на поддръжка, като използвате тази команда:
    
   ** MDEClientAnalyzer.cmd -v**

    За повече информация вижте [Проблеми с компютрите за табло към Microsoft Defender за крайни точки](issues-with-onboarding-machines.md).
