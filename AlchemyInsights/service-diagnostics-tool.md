---
title: Инструмент за диагностика на услуги за виртуален работен плот на Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595457"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Инструмент за диагностика на услуги за виртуален работен плот на Windows

Windows Virtual Desktop (WVD) предлага диагностичен инструмент, който позволява на администраторите да идентифицират грешките чрез един интерфейс. Този инструмент регистрира информация, свързана с диагностиката, всеки път, когато WVD се използва от някого, на когото е присвоена WVD роля. Всеки регистрационен файл съдържа информация за WVD ролята, участваща в дейността, съобщенията за грешки, които се показват по време на сесията, и информацията за клиента и потребителя. Azure Log Analytics може да бъде конфигуриран да заснема регистрационния файл на дейността, създаден от диагностичния инструмент, като изпълните следните стъпки:

1. Създайте работна област log Analytics с [портала на Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Свързване на компютри с Windows към Монитор на Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Получете ИД на работна област и първичния ключ на вашата работна област. Съветникът за настройка се нуждае от тази информация, за да конфигурира правилно агента и да се увери, че може да комуникира с Azure Monitor.

1. [Избутайте диагностични данни в работната област.](https://go.microsoft.com/fwlink/?linkid=2128284) Можете да избутате диагностични данни от вашия WVD клиент към Log Analytics за вашата работна област.

1. [Идентифицирайте и диагностицирайте](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) проблеми, които са вътрешни или външни във връзка с WVD.

За да научите повече за конфигурирането на инструмента за диагностика на услуги за WVD, вижте Използване на анализ на регистрационни файлове за функцията за диагностика.