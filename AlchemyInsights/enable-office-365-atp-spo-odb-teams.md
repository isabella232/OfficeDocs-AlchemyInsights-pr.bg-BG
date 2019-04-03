---
title: Разрешаване на Office 365 АТФ за SharePoint, OneDrive и екипи на Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030886"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Разрешаване на Office 365 разширени заплаха защита за SharePoint онлайн, OneDrive и екипи на Microsoft

1. Отидете на https://protection.office.com и влезте в нея.
2. Изберете **управление на заплахите** > **политика** > **Безопасно прикачени файлове**.
3. Изберете **включване на АТФ за SharePoint, OneDrive и екипи на Microsoft**и след това щракнете върху **Запиши**.
4. (Препоръчва се) Като глобален администратор или администратор на SharePoint Online стартирате кратката команда [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) с **DisallowInfectedFileDownload** параметър, зададен на *true*.
5. (Препоръчва се) [Настройка на предупрежденията](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) за откритите файлове.

> [!NOTE]
> ATP ще НОТ сканиране всеки един файл в SharePoint Online, OneDrive или екипи на Microsoft. Файлове се сканират асинхронно, чрез процес, който използва споделяне и гост дейност събития, умни евристики и заплахата сигнали, за да идентифицира злонамерени файлове. Вижте [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).