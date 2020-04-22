---
title: S/MIME в Outlook в интернет
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764861"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="50ef2-102">Шифровайте имейл съобщенията в Outlook</span><span class="sxs-lookup"><span data-stu-id="50ef2-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="50ef2-103">Шифроването на съобщения на Microsoft 365 е изградено върху управлението на правата на Microsoft за Azure (Azure RMS), което е част от защитата на информацията в Azure.</span><span class="sxs-lookup"><span data-stu-id="50ef2-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="50ef2-104">Ако абонаментът ви включва управление на правата за Azure или защита на информацията в Azure, **не е необходимо да предприемате никакви действия за ръчно разрешаване или активиране** на услугата за управление на правата.</span><span class="sxs-lookup"><span data-stu-id="50ef2-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="50ef2-105">Въз основа на обратна връзка от клиентите, по подразбиране няма да разрешаваме правилата за потока на exchange поща за автоматично шифроване на изходящи имейли, съдържащи определен тип поверителна информация в клиента ви.</span><span class="sxs-lookup"><span data-stu-id="50ef2-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="50ef2-106">Вместо това, ние предоставяме подробни инструкции как можете да го направите сами.</span><span class="sxs-lookup"><span data-stu-id="50ef2-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="50ef2-107">За допълнителна информация относно създаването на транспортно правило за шифроване на поверителна информация [вж.](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="50ef2-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="50ef2-108">Ако използвате Outlook в уеб (по-рано **OWA**): Когато композирате имейл съобщение, просто кликнете **върху Защита** в OWA.</span><span class="sxs-lookup"><span data-stu-id="50ef2-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="50ef2-109">Това ще се прилага "Не препращай" разрешение.</span><span class="sxs-lookup"><span data-stu-id="50ef2-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="50ef2-110">Щракнете върху **Промяна на разрешение** и изберете **Шифроване,** за да шифровате само съобщението.</span><span class="sxs-lookup"><span data-stu-id="50ef2-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="50ef2-111">Ако използвате **клиент а на Outlook**: За да изпратите шифровано съобщение от Outlook 2013 или 2016 или Outlook 2016 за Mac, изберете **Опции** > **разрешения**, след което изберете опцията за защита, която ви трябва.</span><span class="sxs-lookup"><span data-stu-id="50ef2-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="50ef2-112">За да **шифровате автоматично всички имейли,** изпратени до определени получатели или външни партньорски организации, трябва да създадете правило за транспортиране на пощенски поток в Центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="50ef2-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="50ef2-113">Подробни инструкции са дадени в [тази статия за поддръжка](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="50ef2-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

