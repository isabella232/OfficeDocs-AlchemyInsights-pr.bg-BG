---
title: Крайна точка DLP не е разположена на устройството на потребителя
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731276"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Крайна точка DLP не е разположена на устройството на потребителя

Ако настройката за защита от загуба на данни на крайна точка (DLP) не е приложена към устройството на потребителя, уверете се, че отговаряте на тези изисквания:

- Windows 10 x64 компилация 1809 или по-нова версия е инсталирана на устройството.
- Инсталирана е версия 4.18.2009.7 или по-нова версия на злонамерен софтуер.
- Устройството е **едно от** следните:
    
    - Azure Active Directory (Azure AD) присъединен
    - Хибридно присъединяване на Azure AD
    - AAD регистрирано

- За да наложите действия по правилата, се уверете, че браузърът Chromium Edge на Microsoft е инсталиран на устройството с крайна точка.

За допълнителни изисквания за разполагане на DLP за крайна точка вижте [Първи стъпки в предотвратяването на загубата на данни за крайна точка.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)