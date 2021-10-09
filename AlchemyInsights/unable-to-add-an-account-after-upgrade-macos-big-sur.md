---
title: Не можете да добавите акаунт след надстройване до macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506212"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Не можете да добавите акаунт след надстройване до macOS 11.6 Big Sur

След надстройване до macOS 11.6 вашият OneDrive за работа или учебен акаунт или вашият личен акаунт за OneDrive може да не се появи в списъка с акаунти и може да не успеете да влезете във втори акаунт от приложението.

За този проблем е разработена корекция. Първо, определете дали изпълнявате самостоятелната версия или версията на App Store на OneDrive:

- Изберете облака OneDrive в лентата с менюта, > **помощ & Настройки**  >  **Предпочитания**  >  **за**. Ако номерът на версията не включва **(самостоятелен),** имате версията app Store на продукта.

Ако използвате самостоятелната версия на OneDrive, рестартирайте компютъра и OneDrive автоматично актуализира до компилация, където този проблем е решен. Ако искате да инсталирате компилацията ръчно, изтеглете този [файл на.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip), разархивиране на файла и копирайте приложението OneDrive в папката Приложения (като заместите съществуващото приложение OneDrive).

Ако използвате версията app Store, помислете за инсталиране на самостоятелната версия на OneDrive. Тази версия работи по същия начин като версията на App Store, но позволява на Microsoft да предлага актуализации по-бързо на потребителите и ги свързва към версия, която включва корекцията за този проблем.

1. Изтеглете самостоятелната версия на [OneDrive, която включва корекцията.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Разархивиране на файла и копиране на OneDrive в папката "Приложения" (като заместите съществуващото OneDrive приложение).

Ако трябва да използвате версията app Store, изчакайте app Store, за да освободите версия на приложението, която включва корекцията. За съжаление, Microsoft не може да съобщи прогнозна дата, за да бъде издадена фиксирана версия от App Store.

