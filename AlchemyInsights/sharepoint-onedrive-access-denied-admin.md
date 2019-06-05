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
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716636"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Отстраняване на неизправности при съобщения за отказан достъп в центъра за администриране на Sharepoint/OneDrive

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Ако получавате съобщение за отказан, когато се опитвате да отидете до центъра за администриране на Sharepoint/OneDrive достъп, моля уверете се, че можете да <a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">присвоите даден лиценз за потребителя </a>. Ако потребителят има лиценз, ти рамо също правя сигурен те са <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">възложени на администратор роля</a> която достъп на администратор центрове.</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">Този въпрос също може да възникне, когато потребителят е изтрита и създадена отново със същото основно име на потребителя (UPN). Новият акаунт е създаден с помощта на различни PUID (паспорт уникален ИД) стойност. Когато потребителят се опитва да получи достъп до колекция от сайтове или техните OneDrive, потребителят има неправилен PUID. Вторият сценарий включва директория синхронизация с Active Directory организационни единици (OU). Ако потребителите са вече влезли в SharePoint, след това се премества в различни OU и resynced с SharePoint, те могат да срещнат този проблем.</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">За да разрешите този проблем, трябва да възстановите оригиналния UPN със стъпките в статията, <a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">възстановяване на потребител в Office 365</a>.</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">Забележка:</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">Ако OneDrive или SharePoint администратор център не е наличен на множество потребители, които преди това са имали достъп, може да има проблем при временна услуга.&nbsp; </span></span></em> <em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"> <a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">Проверка на услугата здравето таблото</span></a>.</span></em></span></span></p>


