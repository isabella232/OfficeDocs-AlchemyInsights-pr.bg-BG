---
title: Препращане на имейл чрез Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 8f8b0780ebec2911b6698deee25e0fabe83bd9afef5fb3a6ef4c51cccd67fc7c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57898537"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Настройване на многофункционално устройство или приложение за изпращане на имейл

За да научите за вашите възможности и стъпките, вижте [Как се настройва многофункционално устройство или приложение за изпращане на имейл с помощта на Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Ако имате устройство или приложение, които наскоро са спрели да работят, най-често срещаните проблеми са:

- **Грешки, свързани с удостоверяването при използване на изпращане на SMTP удостоверяване на клиент** Наскоро направихме някои промени, свързани с начина на работа на SMTP удостоверяването. За повече информация как да отстраните проблеми, вижте секцията за неуспешно удостоверяване на Коригиране на проблеми с принтери, скенери и [LOB приложения,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)които изпращат имейл чрез Microsoft 365 или Office 365.
- **Приемаме само версията TLS 1.2, докато правим защитена връзка с Office 365** Ако използвате защитена връзка (TLS), уверете се, че вашето устройство на приложението поддържа TLS 1.2. За повече информация вижте Подготовка [за TLS 1.2 в Office 365 и Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
За други проблеми и решения вижте Коригиране на проблеми с принтери, скенери и [LOB приложения,](https://docs.microsoft.com/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)които изпращат имейли чрез Microsoft 365 или Office 365.

За да видите засегнатите устройства, отидете на [Отчет за клиентите с SMTP удостоверяване](https://protection.office.com/mailflow/dashboard).

**Забележка:** Exchange Online не се побира в сценариите за групово изпращане. За да изпратите групов търговски имейл (например бюлетини на клиенти), трябва да използвате доставчици на трети страни, които са специализирани в тези услуги.
