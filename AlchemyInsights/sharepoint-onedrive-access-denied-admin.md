---
title: Отстраняване на неизправности при отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505368"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на неизправности в достъпа отказан съобщения в Центъра за администриране на Sharepoint/OneDrive

Ако получавате съобщение за отказан достъп при опит за преглед на центъра за администриране на Sharepoint/OneDrive, уверете се, че [сте присволи лиценз на потребителя](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ако потребителят има лиценз, трябва също така да се уверите, че му е [присвоена роля](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) на администратор, който може да получи достъп до центровете за администриране.

Този проблем може да възникне, когато потребителят се изтрива и създава отново със същото основно име на потребителя (UPN). Новият акаунт се създава с различна стойност puid (паспорт уникален ИД). Когато потребителят се опита да получите достъп до колекция от сайтове или своя OneDrive, потребителят е неправилен PUID. Втори сценарий включва указатели с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друг ОЕ и resynced SharePoint, те може да се появи този проблем.

За да разрешите този проблем, трябва да възстановите първоначалната UPN стъпки в статията, [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Забележка: Ако OneDrive или център за администриране на SharePoint не е наличен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.  [Проверете таблото за състояние на услугата](https://portal.office.com/adminportal/home#/servicehealth).


