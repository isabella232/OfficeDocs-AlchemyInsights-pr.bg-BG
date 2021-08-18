---
title: Конфигуриране на DLP на крайна точка
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323907"
---
# <a name="configure-endpoint-dlp"></a>Конфигуриране на DLP на крайна точка

DLP на крайна точка на Microsoft ви позволява да разширите възможностите за DLP защита и наблюдение за чувствителна информация на устройства с Windows 10. След като устройствата се регистрират в управлението на устройства, можете да създадете DLP правила, за да приложите защитни действия върху елементи. „Преглед на дейността“ може да се използва за наблюдение на дейността при чувствителни елементи. За повече информация вж. [Регистриране на устройства в управлението на устройства](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

За да започнете с DLP за крайна точка:

- Уверете се, че имате съответния лиценз за ИЕ/абонамент. За повече информация вж. [лицензи за ИЕ/абонаменти](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Проверете разрешенията, необходими за разрешаване на управлението на устройства, достъпа до страницата за регистриране или включване/изключване на наблюдението на устройства. За повече информация вж. [Разрешения](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Регистрирайте устройствата в управлението на устройства, като се следвате процедурата за регистриране на устройства. За повече информация вж. [Регистриране на устройства](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Създайте DLP правила, за да защитите своите чувствителни елементи. За информация вж. [Сценарии за DLP правила за крайна точка](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

За повече информация относно DLP за крайна точка на Microsoft вж. [Научете за защитата от загуба на данни на крайна точка на Microsoft 365 (предварителен преглед)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Важни стъпки за събиране на данни, ако е необходима поддръжка:**

1. Изтегляне [на визуализация на анализатора на клиенти на MDATP](https://aka.ms/betamdatpanalyzer).
1. Изпълнете инструмента като администратор от командния прозорец:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Когато получите подкана с **Въведете броя минути, за да съберете проследявания:** въведете броя минути, необходими за изпълнение на сценария.
1. Изпълнете сценария.

Съберете изходния файл zip, за да дадете на агента по поддръжката.
