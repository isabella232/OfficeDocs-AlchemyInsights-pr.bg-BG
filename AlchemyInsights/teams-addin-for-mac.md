---
title: Teams добавка за Mac
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
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582059"
---
# <a name="teams-add-in-for-mac"></a>Teams добавка за Mac

За да отстраните Teams добавка за потребители на операционната система Mac, изпълнете следните стъпки:

**Стъпка 1:** Ако имате хибридно Exchange локално (изисква се 2016 CU3 или по-нова версия), използвайте инструмента Test-HMA.ps1, за да потвърдите, че хибридното модерно удостоверяване е конфигурирано правилно. За повече информация вижте Проверка [на настройката за модерно хибридно удостоверяване за Outlook за iOS и Android.](https://aka.ms/TestHMAEAS)  

**Забележка** Използвайте формата за UPN адрес (например username@contoso.com [),](mailto:username@contoso.com)а не домейн\потребителско име. Направете това дори за потребители с Exchange Online пощенски кутии.

**Стъпка 2:** Дайте на потребителя да отиде **в "Акаунти за**  >  **инструменти"**... в Outlook за Mac и намерете и изберете акаунта. Уверете се, че потребителското име в списъка е във формат UPN [(например username@contoso.com](mailto:username@contoso.com)).

**Стъпка 3:** Уверете се, че потребителят е лицензиран Microsoft Teams потребител. Потребителят трябва да използва абонамента за Office 365 Mac, версия на продукта 16.24 или по-нова.