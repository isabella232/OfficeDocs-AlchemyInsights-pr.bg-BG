---
title: S/MIME в Outlook в мрежата
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053214"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="a7a64-102">Шифроване на имейл съобщения в Outlook</span><span class="sxs-lookup"><span data-stu-id="a7a64-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="a7a64-103">Office 365 съобщение за шифроване е изградена на управление на правата на Microsoft Azure (Azure RMS), която е част от Azure защита на информацията.</span><span class="sxs-lookup"><span data-stu-id="a7a64-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="a7a64-104">Ако абонаментът ви включва управление на правата на Azure или защита на информацията в Azure, **не е необходимо да предприемете действия за ръчно разрешаване или активиране** на услугата за управление на права.</span><span class="sxs-lookup"><span data-stu-id="a7a64-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="a7a64-105">Въз основа на обратната връзка от клиента, ние вече няма да позволяват правила за пощенски поток на Exchange за автоматично шифроване на изходящ имейл, съдържащ определен тип чувствителна информация в клиента по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="a7a64-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="a7a64-106">Вместо това ние предоставяме подробни инструкции как можете да направите това сами.</span><span class="sxs-lookup"><span data-stu-id="a7a64-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="a7a64-107">За допълнителна информация относно създаването на транспортно правило за шифроване на поверителна информация вижте [тази статия](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="a7a64-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="a7a64-108">Ако използвате Outlook в уеб (бивш **OWA**): при съставяне на имейл съобщение, просто щракнете върху **защита** в OWA.</span><span class="sxs-lookup"><span data-stu-id="a7a64-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="a7a64-109">Това ще се прилага "не напред" разрешение.</span><span class="sxs-lookup"><span data-stu-id="a7a64-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="a7a64-110">Кликнете върху **Промяна на разрешенията** и изберете **шифроване** , за да шифровате само съобщението.</span><span class="sxs-lookup"><span data-stu-id="a7a64-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="a7a64-111">Ако използвате **Outlook клиент**: за да изпратите шифровано съобщение от Outlook 2013 или 2016, или Outlook 2016 за Mac, изберете **Опции** > **разрешения**, след което изберете опцията за защита, която трябва.</span><span class="sxs-lookup"><span data-stu-id="a7a64-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="a7a64-112">За да **шифровате автоматично всички имейли** , изпратени до определени получатели или организации на външни партньори, трябва да създадете правило за транспортиране на пощенски поток в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7a64-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="a7a64-113">Подробни инструкции са предоставени в [тази статия за поддръжка](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="a7a64-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

