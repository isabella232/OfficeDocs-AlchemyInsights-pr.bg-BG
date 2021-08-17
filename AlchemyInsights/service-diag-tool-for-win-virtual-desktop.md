---
title: Инструмент за диагностика на услуги за Windows виртуален работен плот
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052375"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Инструмент за диагностика на услуги за Windows виртуален работен плот

Windows Виртуалният работен плот (WVD) предлага диагностичен инструмент, който позволява на администраторите да идентифицират грешките чрез един интерфейс. Този инструмент регистрира информация, свързана с диагностиката, всеки път, когато WVD се използва от някого, на когото е присвоена WVD роля. Всеки регистрационен файл съдържа информация за WVD ролята, участваща в дейността, съобщенията за грешки, които се показват по време на сесията, и информацията за клиента и потребителя. Azure Log Analytics може да бъде конфигуриран да заснема регистрационния файл за дейността, създаден от диагностичния инструмент. Ето как:

1. Създайте работна област log Analytics с [портала на Azure](https://go.microsoft.com/fwlink/?linkid=2129500) или [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Свързване Windows компютри към Монитор на Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Получете ИД на работна област и първичния ключ на вашата работна област. Съветникът за настройка се нуждае от тази информация, за да конфигурира правилно агента и да се увери, че може да комуникира с Azure Monitor.
1. [Избутайте диагностични данни в работната област.](https://go.microsoft.com/fwlink/?linkid=2128284) Можете да избутате диагностични данни от вашия WVD клиент към Log Analytics за вашата работна област.
1. [Идентифицирайте и диагностицирайте проблеми,](https://go.microsoft.com/fwlink/?linkid=2128338) които са вътрешни или външни във връзка с WVD.

За да научите повече за конфигурирането на инструмента за диагностика на услуги за WVD, вижте Използване на [анализ на регистрационни файлове за функцията за диагностика](https://go.microsoft.com/fwlink/?linkid=2128084).
