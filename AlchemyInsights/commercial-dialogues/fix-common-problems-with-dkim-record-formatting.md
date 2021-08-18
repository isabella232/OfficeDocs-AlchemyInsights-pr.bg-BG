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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323979"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Коригиране на често срещани проблеми с форматирането на DKIM записи

Повечето проблеми с настройването на DKIM са свързани с неправилни DNS записи.

За да коригирате проблемите с настройването на DKIM, проверете дали DKIM CNAME **записът** (а не TXT запис) е форматиран правилно. За повече информация вижте Какво [трябва да направите, за да настроите ръчно DKIM в Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Ако имате нужда от помощ за DNS записите като цяло, вижте [Създаване на DNS записи при всеки доставчик на DNS хостинг за Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Забележка:** След като създадете или актуализирате своите DKIM DNS записи в dns хостинг услугата за вашия домейн, ще трябва да изчакате DNS записите да се разпространяват.
