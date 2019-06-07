---
title: Отстраняване на неизправности при съобщения за отказан достъп
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760330"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на неизправности при съобщения за отказан достъп в центъра за администриране на Sharepoint/OneDrive

Ако получавате съобщение за отказан, когато се опитвате да отидете до центъра за администриране на Sharepoint/OneDrive достъп, моля уверете се, че можете да [присвоите даден лиценз за потребителя](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Ако потребителят има лиценз, ти рамо също правя сигурен те са [възложени на администратор роля](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) която достъп на администратор центрове.

Този въпрос също може да възникне, когато потребителят е изтрита и създадена отново със същото основно име на потребителя (UPN). Новият акаунт е създаден с помощта на различни PUID (паспорт уникален ИД) стойност. Когато потребителят се опитва да получи достъп до колекция от сайтове или техните OneDrive, потребителят има неправилен PUID. Вторият сценарий включва директория синхронизация с Active Directory организационни единици (OU). Ако потребителите са вече влезли в SharePoint, след това се премества в различни OU и resynced с SharePoint, те могат да срещнат този проблем.

За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в статията, [възстановяване на потребител в Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Забележка: Ако OneDrive или SharePoint администратор център не е наличен на множество потребители, които преди това са имали достъп, може да има проблем при временна услуга.  [Проверете услуги здравето на таблото](https://portal.office.com/adminportal/home#/servicehealth).


