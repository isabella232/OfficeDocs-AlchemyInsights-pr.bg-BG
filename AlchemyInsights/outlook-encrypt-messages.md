---
title: S/MIME в Outlook в мрежата
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752849"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="6d91a-102">Шифроване на имейл съобщения в Outlook</span><span class="sxs-lookup"><span data-stu-id="6d91a-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="6d91a-103">Office 365 съобщение за шифроване е изградена на управление на правата на Microsoft Azure (Azure RMS), която е част от Azure защита на информацията.</span><span class="sxs-lookup"><span data-stu-id="6d91a-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="6d91a-104">Ако абонаментът ви включва управление на правата на Azure или защита на информацията в Azure, **не е необходимо да предприемете действия за ръчно разрешаване или активиране** на услугата за управление на права.</span><span class="sxs-lookup"><span data-stu-id="6d91a-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="6d91a-105">Въз основа на обратната връзка от клиента, ние вече няма да позволяват правила за пощенски поток на Exchange за автоматично шифроване на изходящ имейл, съдържащ определен тип чувствителна информация в клиента по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="6d91a-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="6d91a-106">Вместо това ние предоставяме подробни инструкции как можете да направите това сами.</span><span class="sxs-lookup"><span data-stu-id="6d91a-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="6d91a-107">За допълнителна информация относно създаването на транспортно правило за шифроване на поверителна информация вижте [тази статия](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="6d91a-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="6d91a-108">Ако използвате Outlook в уеб (бивш **OWA**): при съставяне на имейл съобщение, просто щракнете върху **защита** в OWA.</span><span class="sxs-lookup"><span data-stu-id="6d91a-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="6d91a-109">Това ще се прилага "не напред" разрешение.</span><span class="sxs-lookup"><span data-stu-id="6d91a-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="6d91a-110">Кликнете върху **Промяна на разрешенията** и изберете **шифроване** , за да шифровате само съобщението.</span><span class="sxs-lookup"><span data-stu-id="6d91a-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="6d91a-111">Ако използвате **Outlook клиент**: за да изпратите шифровано съобщение от Outlook 2013 или 2016, или Outlook 2016 за Mac, изберете **Опции** > **разрешения**, след което изберете опцията за защита, която трябва.</span><span class="sxs-lookup"><span data-stu-id="6d91a-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="6d91a-112">За да **шифровате автоматично всички имейли** , изпратени до определени получатели или организации на външни партньори, трябва да създадете правило за транспортиране на пощенски поток в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d91a-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="6d91a-113">Подробни инструкции са предоставени в [тази статия за поддръжка](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="6d91a-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

