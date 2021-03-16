---
title: Премахване на услугата за фон за Microsoft Search в Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816072"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Премахване на услугата за фон за Microsoft Search в Bing

За да премахнете услугата за фон за Microsoft Search в Bing, можете да изпробвате следните корективни мерки:

1. За да се върнете към първоначалните настройки на системата за търсене, направете следните неща:

    на. Превключване на превключвателя за **използване на Bing като [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) търсачка по подразбиране**.

    b. [Отидете в центъра за администриране на Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) и изчистете настройката, която засяга всички потребители във вашата организация.

2. За да премахнете услугата за фон от отделно устройство, направете следните задачи:

    на. Изберете **Control Panel > програми > програми и функции**.

    b. Щракнете с десния бутон върху **Microsoft Search в Bing** под списъка с инсталирани програми, след което щракнете върху **деинсталирай**.

3. За да премахнете услугата за заден фон от множество устройства във вашата организация, влезте като администратор и изпълнете следната команда в скрипт: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
