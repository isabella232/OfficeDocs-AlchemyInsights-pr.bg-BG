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
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940664"
---
# <a name="teams-add-in-for-mac"></a>Teams добавка за Mac

За да отстраните Teams добавка за потребители на операционната система Mac, изпълнете следните стъпки:

**Стъпка 1:** Ако имате хибридно Exchange локално (изисква се 2016 CU3 или по-нова версия), използвайте инструмента Test-HMA.ps1, за да потвърдите, че хибридното модерно удостоверяване е конфигурирано правилно. За повече информация вижте Проверка [на настройката за модерно хибридно удостоверяване за Outlook за iOS и Android.](https://aka.ms/TestHMAEAS)  

**Забележка** Използвайте формата за UPN адрес (например username@contoso.com [),](mailto:username@contoso.com)а не домейн\потребителско име. Направете това дори за потребители с Exchange Online пощенски кутии.

**Стъпка 2:** Дайте на потребителя да отиде **в "Акаунти за**  >  **инструменти"**... в Outlook за Mac и намерете и изберете акаунта. Уверете се, че потребителското име в списъка е във формат UPN [(например username@contoso.com](mailto:username@contoso.com)).

**Стъпка 3:** Уверете се, че потребителят е лицензиран Microsoft Teams потребител. Потребителят трябва да използва абонамента за Office 365 Mac, версия на продукта 16.24 или по-нова.