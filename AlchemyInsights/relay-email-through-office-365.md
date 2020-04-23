---
title: Препращане на имейл чрез Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785184"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="37cd6-102">Настройване на многофункционално устройство или приложение за изпращане на имейл</span><span class="sxs-lookup"><span data-stu-id="37cd6-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="37cd6-103">За да научите за вашите възможности и стъпките, вижте [Как се настройва многофункционално устройство или приложение за изпращане на имейл с помощта на Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="37cd6-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="37cd6-104">**Забележка:** Ако имате устройство или приложение, което наскоро е спряло да работи, имайте предвид, че наскоро сме започнали [да забраняваме шифъра 3DES](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption), както е планирано.</span><span class="sxs-lookup"><span data-stu-id="37cd6-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="37cd6-105">За да видите засегнатите устройства, отидете на [Отчет за клиентите с SMTP удостоверяване](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="37cd6-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="37cd6-106">Често срещаните грешки може да са подобни на: неуспех/грешка при удостоверяване на автентичност, TLS неуспех/грешка, грешка в алгоритъма на шифъра, несъответствие в алгоритъма или прекъсната връзка.</span><span class="sxs-lookup"><span data-stu-id="37cd6-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="37cd6-107">За решаване на проблема:</span><span class="sxs-lookup"><span data-stu-id="37cd6-107">To resolve the issue:</span></span>
 - <span data-ttu-id="37cd6-108">**Windows Server 2003 IIS SMTP няма да работи повече – по-новата версия на Windows е задължителна.**</span><span class="sxs-lookup"><span data-stu-id="37cd6-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="37cd6-109">Моля, консултирайте се с доставчика на вашето приложение или устройство, за да проверите дали се поддържа модерен шифър или, дали е налична актуализация.</span><span class="sxs-lookup"><span data-stu-id="37cd6-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
