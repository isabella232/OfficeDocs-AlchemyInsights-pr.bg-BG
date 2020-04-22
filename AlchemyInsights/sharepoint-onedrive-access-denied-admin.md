---
title: Отстраняване на отказан достъп съобщения
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758364"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на отказан достъп съобщения в центъра за администриране на SharePoint/OneDrive

Ако получавате съобщение за отказан достъп при опит за преглед на център за администриране на Sharepoint/OneDrive, моля, уверете се, че [присвоите лиценз на потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ако потребителят има лиценз, трябва също да се уверите, че им е [присвоена администраторска роля,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) която да има достъп до центровете за администриране.

Този проблем може да възникне, когато потребител е изтрит и повторно създаден със същото основно потребителско име (UPN). Новият акаунт се създава чрез различна стойност на PUID (уникален ид на паспорт). Когато потребителят се опита да получите достъп до колекция от сайтове или oneDrive, потребителят има неправилен PUID. Втори сценарий включва синхронизиране на директории с Active Directory организационна единица (ОЕ). Ако потребителите вече са влезли в SharePoint и след това се преместват в друг OU и resynced с SharePoint, те могат да възникнат този проблем.

За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в [статията, възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Забележка: Ако OneDrive или център за администриране на SharePoint не е достъпен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.  [Проверете таблото за изправност на услугата](https://portal.office.com/adminportal/home#/servicehealth).


