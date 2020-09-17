---
title: Възникна грешка при проверката на грешката на маркера за достъп по време на настолната версия на компютъра
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783540"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Грешка "Възникна грешка при проверка на маркера за достъп" по време на насложения в настолен анализ

Тази грешка се наблюдава обикновено при изтичане на маркера за удостоверяване. Обикновено обновяването на страницата обновява маркера. Обаче този проблем може да продължи, ако има някакви правила за условен достъп, които са приложени към акаунта, който се използва за настолните анализи на борда. Можете да прегледате влизане в Azure AD в регистрационни файлове в портала на Azure, за да видите дали има неизправности при влизане, за да се използва акаунтът за настолната версия на анализи.

За повече информация относно условния достъп отидете на [планиране на разполагане на условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).