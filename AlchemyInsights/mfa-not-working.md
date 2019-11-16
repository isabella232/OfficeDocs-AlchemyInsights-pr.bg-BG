---
title: Проблеми с МФП
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768826"
---
# <a name="issues-with-azure-mfa"></a>Проблеми с Azure МФП
Има няколко неща, за да проверите дали потребителите не могат да влязат с помощта на многофакторно удостоверяване (МФП)

1. Засегнатите потребител може да бъде блокиран в Azure Active Directory портал. Ако това е така, опитите за удостоверяване за този конкретен потребител ще бъдат автоматично отказани. [Следвайте стъпките в тази статия, за да ги деблокирате.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ако деблокирането на потребителя не помогна или потребителят не е блокиран, можете да опитате да нулирате МФП за потребителя и те ще мине през процеса на записване отново. [Моля, следвайте стъпките в тази статия.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ако това е първият път, когато сте разрешили МФП и вашите потребители са в състояние да влезете в не-браузъри клиенти като Outlook, Skype и т. н., може би ЛОТАРИНГИЯ (Active Directory удостоверяване библиотека) не е разрешена на вашия абонамент за O365. В този случай ще трябва да се свържете с Exchange Online PowerShell и изпълнете тази команда:  *Set-Организацияconfig-OAuth2ClientProfileEnabled: $True*