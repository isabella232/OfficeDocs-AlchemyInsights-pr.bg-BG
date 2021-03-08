---
title: Регистрационни файлове с пароли
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523610"
---
# <a name="password-logs"></a>Регистрационни файлове с пароли

**Имам проблеми при достъп до регистрационни файлове за проверка на нулиране на пароли**

За отстраняване на проблеми, свързани с достъпа до регистрите за проверка на нулиране на пароли, изпълнете следната стъпка:

Уверете се, че сте упълномощени да преглеждате регистрационни файлове за проверка. 

Разрешават се само следните роли:
 - Глобален администратор
 - Администратор по защитата
 - Четец за защита

**Искам да видя всички събития за проверка на нулирането на пароли от момента на първоначалното разполагане**

Събития за нулиране на паролата/регистрация на 120 000 се съхраняват в отчетите на последните 30 дни. Това максимално ограничение се отнася за потребителския интерфейс при изтегляне на CSV файла. събития за 1 000 000 са достъпни чрез PowerShell.
За повече информация вижте връзките по-долу:

- [Събития за самостоятелно нулиране на пароли от отчетите на Azure AD и API за събития](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Как да изтеглите бързо събития за регистрация на нулиране на пароли с PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Искам да разбера повече за възможностите за отчитане на нулиране на пароли**

Проверете кой е регистрирал или нулирал паролите с регистрационни файлове за проверка на парола на Azure AD в портала на Azure под **потребители и групи**.
За повече информация вижте следните връзки:

- [Обзор на отчетите за нулиране на паролата](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Как да преглеждате отчетите за нулиране на паролата в портала на Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Събития за самостоятелно нулиране на пароли от отчетите на Azure AD и API за събития](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Как да изтеглите бързо събития за регистрация на нулиране на пароли с PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


