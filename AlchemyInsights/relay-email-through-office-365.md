---
title: Препращане на имейл чрез Microsoft 365
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
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117972"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="aabe2-102">Настройване на многофункционално устройство или приложение за изпращане на имейл</span><span class="sxs-lookup"><span data-stu-id="aabe2-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="aabe2-103">За да научите за вашите възможности и стъпките, вижте [Как се настройва многофункционално устройство или приложение за изпращане на имейл с помощта на Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="aabe2-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="aabe2-104">Ако имате устройство или приложение, които наскоро са спрели да работят, най-често срещаните проблеми са:</span><span class="sxs-lookup"><span data-stu-id="aabe2-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="aabe2-105">**Грешки, свързани с удостоверяването при използване на изпращане на SMTP удостоверяване на клиент** Наскоро направихме някои промени, свързани с начина на работа на SMTP удостоверяването.</span><span class="sxs-lookup"><span data-stu-id="aabe2-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="aabe2-106">За повече информация как да отстраните проблеми, вижте секцията за неуспешно удостоверяване на Коригиране на проблеми с принтери, скенери и [LOB приложения,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)които изпращат имейл чрез Microsoft 365 или Office 365.</span><span class="sxs-lookup"><span data-stu-id="aabe2-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="aabe2-107">**Приемаме само версията TLS 1.2, докато правим защитена връзка с Office 365** Ако използвате защитена връзка (TLS), уверете се, че вашето устройство на приложението поддържа TLS 1.2.</span><span class="sxs-lookup"><span data-stu-id="aabe2-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="aabe2-108">За повече информация вижте Подготовка [за TLS 1.2 в Office 365 и Office 365 GCC.](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="aabe2-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="aabe2-109">За други проблеми и решения вижте Коригиране на проблеми с принтери, скенери и [LOB приложения,](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)които изпращат имейл чрез Microsoft 365 или Office 365.</span><span class="sxs-lookup"><span data-stu-id="aabe2-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="aabe2-110">За да видите засегнатите устройства, отидете на [Отчет за клиентите с SMTP удостоверяване](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="aabe2-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="aabe2-111">**Забележка:** Exchange Online не се побира в сценариите за групово изпращане.</span><span class="sxs-lookup"><span data-stu-id="aabe2-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="aabe2-112">За да изпратите групов търговски имейл (например бюлетини на клиенти), трябва да използвате доставчици на трети страни, които са специализирани в тези услуги.</span><span class="sxs-lookup"><span data-stu-id="aabe2-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
