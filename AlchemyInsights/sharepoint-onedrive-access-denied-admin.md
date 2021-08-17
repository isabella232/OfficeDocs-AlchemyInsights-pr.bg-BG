---
title: Отстраняване на неизправности с отказан достъп до съобщения
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085217"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на неизправности с отказан достъп до съобщения в sharepoint/OneDrive център за администриране

Ако получавате съобщение за отказан достъп, когато се опитвате да отидете до център за администриране на Sharepoint/OneDrive, трябва да дадете [лиценз на потребителя](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ако потребителят има лиценз, трябва също да се уверите, че му е [присвоена администраторска роля, която](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) има достъп до центровете за администриране.

Този проблем може да възникне и когато потребител бъде изтрит и създаден отново със същото основно потребителско име (UPN). Новият акаунт се създава с помощта на различна стойност на PUID (уникален ИД за паспорт). Когато потребителят се опита да получи достъп до колекция от сайтове или OneDrive, потребителят има неправилен PUID. Вторият сценарий включва синхронизиране на справочника с организационна единица на Active Directory (OU). Ако потребителите вече са влезли в SharePoint и след това са преместени в друг OU и са пренасочени с SharePoint, те може да възникнат този проблем.

За да разрешите този проблем, трябва да възстановите първоначалния UPN със стъпките в статията, [Възстановяване на потребител в Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Забележка: Ако център OneDrive или SharePoint за администриране не е наличен за няколко потребители, които преди това са имали достъп, може да има временен проблем с услугата.  [Проверете таблото за изтежне на услугата](https://portal.office.com/adminportal/home#/servicehealth).


