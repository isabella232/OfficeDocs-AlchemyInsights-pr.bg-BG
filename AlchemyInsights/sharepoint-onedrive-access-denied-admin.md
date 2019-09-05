---
title: Отстраняване на съобщения за отказан достъп
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751265"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на съобщения за отказан достъп в SharePoint/OneDrive център за администриране

Ако получавате съобщение за отказан достъп при опит за преглеждане в център за администриране на SharePoint/OneDrive, моля, уверете се, че [присвоявате лиценз на потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ако потребителят има лиценз, трябва да се уверите, че те са [присвоени администраторски роля](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , която има достъп до центровете за администриране.

Този проблем може да възникне, когато потребителят се изтрива и създава отново със същото основно потребителско име (UPN). Нов акаунт се създава с помощта на различен PUID (паспорт Еднозначен ID) стойност. Когато потребителят се опита да получите достъп до колекция от сайтове или техните OneDrive, потребителят е неправилен PUID. Втори сценарий включва указатели с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друга ОЕ и повторно синхронизиране с SharePoint, те могат да възникнат този проблем.

За да разрешите този проблем, трябва да възстановите оригиналния UPN стъпки в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Забележка: Ако OneDrive или център за администриране на SharePoint не е достъпен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.  [Проверете таблото за изправността на услугата](https://portal.office.com/adminportal/home#/servicehealth).


