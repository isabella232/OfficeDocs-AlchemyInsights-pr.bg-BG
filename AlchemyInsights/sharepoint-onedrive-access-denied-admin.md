---
title: Отстраняване на неизправности при отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767641"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на проблеми с отказан достъп на съобщения в центъра за администриране на SharePoint/OneDrive

Ако получавате съобщение за отказан достъп, когато се опитвате да отидете в център за администриране на SharePoint/OneDrive, се уверете, че сте [задали лиценз на потребителя](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ако потребителят има лиценз, трябва също да се уверите, че му е [присвоена административна роля](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , която може да получи достъп до центровете за администриране.

Този проблем може да възникне и когато потребителят бъде изтрит и пресъздаден със същото основно потребителско име (UPN). Новият акаунт се създава с помощта на различна стойност на PUID (уникален ИД за Passport). Когато потребителят се опитва да получи достъп до колекция от сайтове или техния OneDrive, потребителят има неправилни PUID. Вторият сценарий включва синхронизирането на справочен указател с организационната единица за Active Directory (OU). Ако потребителите вече са влезли в SharePoint, а след това бъдат преместени в друга ОЕ и да се синхронизират с SharePoint, може да изпитате този проблем.

За да отстраните този проблем, трябва да възстановите първоначалния UPN със стъпките в статията [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Забележка: Ако един център за администриране на OneDrive или SharePoint не е достъпен за множество потребители, които преди това са имали достъп, е възможно да има временен проблем с услугата.  [Проверете таблото за изправност на услугите](https://portal.office.com/adminportal/home#/servicehealth).


