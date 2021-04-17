---
title: Икона за календар, която не се показва в Teams клиента
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819942"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Икона за календар, която не се показва в Teams клиента

Разделът „Календар“ в Teams изисква достъп до пощенската кутия на Exchange чрез Exchange Web Services. Пощенската кутия на Exchange може да бъде онлайн или локална. За онлайн потребители, които не виждат раздела „Календар“, уверете се, че те[имат лиценз за пощенска кутия на Exchange Online и пощенската кутия е разрешена](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Ако потребителят има валидна пощенска кутия в Exchange Online, но все още не може да види раздела „Календар“, е възможно да се сблъскате с проблем в мрежата. Използвайте инструмента [Анализатор за отдалечено свързване на Microsoft](https://testconnectivity.microsoft.com/) и стартирайте **Тестовете за свързване на Microsoft Exchange Web Services** за засегнатия потребител.

Накрая проверете приложенията за [Teams – правила за настройка на приложения](https://admin.teams.microsoft.com/policies/app-setup), за да се гарантира, че приложението за календар не е премахнато от правилата, приложени към потребителя (най-вероятно **глобален (по подразбиране за организацията)**.

Ако вашите потребители са разположени локално, трябва да потвърдите, че конфигурацията на хибридните ви системи е здрава. Използвайте [Съветника за конфигуриране на хибридно разполагане](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) за отстраняване на неизправностите.

Обърнете внимание, че [Teams изисква Exchange 2016 CU3 или по-нова версия](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
