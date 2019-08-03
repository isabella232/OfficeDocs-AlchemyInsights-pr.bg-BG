---
title: Проблеми с МВНР
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250154"
---
# <a name="issues-with-mfa"></a>Проблеми с МВНР
Има няколко неща, за да проверите дали потребителите не мога да вляза с помощта на удостоверяване (МВНР)

1. Променения потребител може да бъде блокиран в Azure Active Directory портал. Ако случаят е такъв, удостоверяване се опитва за това автоматично ще бъдат отказани конкретен потребител. [Моля, следвайте стъпките в тази статия, за да ги деблокирате.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Ако отблокирате потребител не помогне или потребителят не е блокирана можете да опитате да възстановите МВНР за потребителя и те ще преминат през процеса на записвам отново. [Моля, следвайте стъпките в тази статия.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Ако това е първи път разрешен МВРХ и вашите потребители са в състояние да влезете в не-браузъри клиенти като Outlook, Skype и т.н., може би ADAL (Active Directory удостоверяване библиотека) не е разрешена на абонамента си O365. В този случай ще трябва да се свърже с Exchange Online Powershell и да изпълните тази кратка команда:  *комплект-OrganizationConfig-OAuth2ClientProfileEnabled: $true*