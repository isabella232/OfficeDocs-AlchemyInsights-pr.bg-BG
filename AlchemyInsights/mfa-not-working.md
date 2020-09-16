---
title: Проблеми с МВНР
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755120"
---
# <a name="issues-with-azure-mfa"></a>Проблеми с Azure МВНР
Има няколко неща, които трябва да проверите дали потребителите не могат да влизат, като използват многофакторно удостоверяване (МВНР)

1. Засегнатите потребители могат да бъдат блокирани в Azure Active Directory Portal. Ако това е така, опитите за удостоверяване за този конкретен потребител ще бъдат отхвърлени автоматично. [Моля, следвайте стъпките в тази статия, за да ги разблокирате.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ако разблокирането на потребителя не е помогнало или потребителят не е блокиран, можете да се опитате да нулирате МВНР за потребителя и той отново ще премине през процеса на записване. [Моля, следвайте стъпките в тази статия.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ако това е първият път, когато сте активирали МВНР и вашите потребители не могат да влязат в клиенти, които не са браузъри, като например Outlook, Skype и т. н., може би ADAL (библиотека за удостоверяване на Active Directory) не е разрешена за вашия абонамент за O365. В този случай ще трябва да се свържете с PowerShell на Exchange Online и да изпълните тази кратка команда:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*