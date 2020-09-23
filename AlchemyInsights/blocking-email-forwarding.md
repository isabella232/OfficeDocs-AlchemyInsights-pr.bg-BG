---
title: 726, който блокира препращането на имейли
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219844"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="5b4cc-102">Блокиране или разблокиране на препращане на имейли</span><span class="sxs-lookup"><span data-stu-id="5b4cc-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="5b4cc-103">За да разрешите или забраните препращането на имейли за конкретна пощенска кутия, вижте [Конфигуриране на препращане на имейл](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5b4cc-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="5b4cc-104">На ниво клиент контролата за външно препращане се изпълнява чрез правилата за изходящи спам.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="5b4cc-105">Ако е зададено на изкл. или автоматично, може да блокира препращането на имейли с отказания достъп "550 5.7.520, вашата организация не разрешава външна препращане".</span><span class="sxs-lookup"><span data-stu-id="5b4cc-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="5b4cc-106">Впоследствие, ако е зададено препращане на блокирането, това е грешката, която вашите потребители ще видят.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="5b4cc-107">Ако препращането е блокирано, уверете се, че правилата са конфигурирани така, че да позволяват външни препращане.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="5b4cc-108">Можете да проверите правилата за изходящ филтър за нежелана поща от центъра за защита и съответствие или като изпълните командата get-HostedOutboundSpamFilterPolicy | FL име, AutoForwardingMode.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="5b4cc-109">Ако искате да зададете блокиране на автоматичното препращане, същата команда ще ви покаже състоянието на правилата сега.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="5b4cc-110">Забележка: препоръчително е да запазите неактивираните външни автоматично препращане на правилата за изходящия филтър по подразбиране и да му разрешите само за потребителите, които имат нужда от външно препращане, като създадат правила по избор за тези потребители.</span><span class="sxs-lookup"><span data-stu-id="5b4cc-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="5b4cc-111">Можете да прочетете повече за [конфигурирането на външно препращане на имейли в Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="5b4cc-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>