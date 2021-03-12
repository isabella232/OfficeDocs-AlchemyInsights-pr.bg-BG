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
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="88b9f-102">Коригиране на често срещани проблеми с форматирането на запис на DKIM</span><span class="sxs-lookup"><span data-stu-id="88b9f-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="88b9f-103">Повечето проблеми при настройването на DKIM се отнасят до неправилни DNS записи.</span><span class="sxs-lookup"><span data-stu-id="88b9f-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="88b9f-104">За да коригирате проблеми с настройката на DKIM, се уверете, че CNAME записът на DKIM (**не** TXT запис) е форматиран правилно.</span><span class="sxs-lookup"><span data-stu-id="88b9f-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="88b9f-105">За повече информация вижте [Какво трябва да направите, за да настроите ръчно DKIM в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="88b9f-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="88b9f-106">Ако имате нужда от помощ за DNS записите като цяло, вижте [Създаване на DNS записи при доставчик на DNS хостинг за Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="88b9f-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="88b9f-107">След като създадете или актуализирате вашите DNS записи за DKIM в DNS хостинг услугата за вашия домейн, ще трябва да изчакате DNS записите да се разпространят.</span><span class="sxs-lookup"><span data-stu-id="88b9f-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
