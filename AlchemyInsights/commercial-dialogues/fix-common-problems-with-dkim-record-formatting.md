---
title: Коригиране на често срещани проблеми с форматирането на запис на DKIM
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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743890"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Коригиране на често срещани проблеми с форматирането на запис на DKIM

Повечето проблеми при настройването на DKIM се отнасят до неправилни DNS записи.

За да коригирате проблеми с настройката на DKIM, се уверете, че CNAME записът на DKIM (**не** TXT запис) е форматиран правилно. За повече информация вижте [Какво трябва да направите, за да настроите ръчно DKIM в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Ако имате нужда от помощ за DNS записите като цяло, вижте [Създаване на DNS записи при доставчик на DNS хостинг за Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).

> [!NOTE]
> След като създадете или актуализирате вашите DNS записи за DKIM в DNS хостинг услугата за вашия домейн, ще трябва да изчакате DNS записите да се разпространят.
