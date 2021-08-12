---
title: Възникна грешка при проверка на грешката в маркера за достъп по време на настолната версия на Analytics на борда
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946604"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Грешка "Възникна грешка при проверка на маркера за достъп" по време на таблото на Настолните анализи

Тази грешка обикновено се наблюдава, когато маркерът за удостоверяване изтече. Обикновено обновяването на страницата обновява маркера. Този проблем обаче може да продължи, ако има правила за условен достъп, приложени към акаунта, който се използва за настолни анализи на компютъра. Можете да прегледате регистрационните файлове за влизане в Azure AD в портала на Azure, за да видите дали има грешки при влизане за акаунта, който се използва за настолни анализи.

За повече информация относно условен достъп посетете Планиране [на разполагането на вашия условен достъп](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).