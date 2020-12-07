---
title: Конфигуриране на настройките на правилата за Microsoft Edge в Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583186"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="8cec4-102">Конфигуриране на настройките на правилата за Microsoft Edge в Windows</span><span class="sxs-lookup"><span data-stu-id="8cec4-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="8cec4-103">За да конфигурирате настройките за правилата и управляваните актуализации за Microsoft Edge, използвайте обекти за групови правила (GPOs).</span><span class="sxs-lookup"><span data-stu-id="8cec4-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="8cec4-104">Можете също да осигурите правила чрез системния регистър; Това може да е подходящо за (1) устройства с Windows, които са се присъединили към домейн на Microsoft Active Directory и за (2) Windows 10 Pro и Enterprise инстанции, записани за управление на устройства в Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8cec4-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="8cec4-105">За да конфигурирате Microsoft Edge с помощта на GPOs, направете следното:</span><span class="sxs-lookup"><span data-stu-id="8cec4-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="8cec4-106">Към централния магазин на груповите правила във вашия домейн на Active Directory или към папката на шаблона за дефиниция на правилата на отделни компютри инсталирайте всички административни шаблони, които добавят правила и настройки за Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="8cec4-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="8cec4-107">Конфигурирайте конкретните правила, които искате да зададете.</span><span class="sxs-lookup"><span data-stu-id="8cec4-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="8cec4-108">За да научите повече, вижте [Конфигуриране на настройките за правилата за Microsoft Edge в Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="8cec4-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
