---
title: Коригиране на често срещани проблеми с форматирането на DKIM записи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930050"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Коригиране на често срещани проблеми с форматирането на DKIM записи

Повечето проблеми с настройването на DKIM са свързани с неправилни DNS записи.

За да коригирате проблемите с настройването на DKIM, проверете дали DKIM CNAME **записът** (а не TXT запис) е форматиран правилно. За повече информация вижте Какво [трябва да направите, за да настроите ръчно DKIM в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ако имате нужда от помощ за DNS записите като цяло, вижте [Създаване на DNS записи при всеки доставчик на DNS хостинг за Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> След като създадете или актуализирате своите DKIM DNS записи в DNS хостинг услугата за вашия домейн, ще трябва да изчакате DNS записите да се разпространяват.
