---
title: Добавка за Teams за Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670317"
---
# <a name="teams-add-in-for-mac"></a>Добавка за Teams за Mac

За да отстраните добавка за липсващи екипи за потребители на операционна система Mac, изпълнете следните стъпки:

**Стъпка 1:** Ако имате хибридно разполагане на Exchange (2016 CU3 или по-нова версия), използвайте инструмента за Test-HMA.ps1, за да потвърдите, че хибридното модерно удостоверяване е конфигурирано правилно. За повече информация вижте [проверка на хибридно модерно удостоверяване за Outlook за IOS и Android](https://aka.ms/AA980zq).  

**Забележка** Използвайте формата UPN адрес (например [username@contoso.com](mailto:username@contoso.com)), а не domain\username. Направете това дори за потребители с пощенски кутии на Exchange Online.

**Стъпка 2:** Помолете потребителя да премине към **инструменти**за  >  **акаунти**... в Outlook for Mac и намерете и изберете акаунта. Уверете се, че потребителското име в списъка е в UPN формат (например [username@contoso.com](mailto:username@contoso.com)).

**Стъпка 3:** Уверете се, че потребителят е лицензиран потребител на Microsoft Teams. Потребителят трябва да използва абонамента за Office 365 for Mac, версия на продукта 16,24 или по-нова.