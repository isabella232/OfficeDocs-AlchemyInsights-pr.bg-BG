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
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511497"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="7ce66-102">Шифроване на имейл съобщения в Outlook</span><span class="sxs-lookup"><span data-stu-id="7ce66-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="7ce66-103">Шифроването на съобщения на Microsoft 365 е изградено върху Microsoft Azure управление на правата (Azure RMS), който е част от защитата на информацията в Azure.</span><span class="sxs-lookup"><span data-stu-id="7ce66-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="7ce66-104">Ако вашият абонамент включва Управление на правата на Azure или Защита на информацията в Azure, **не е необходимо да предприемате никакви действия, за да активирате ръчно** услугата за управление на правата.</span><span class="sxs-lookup"><span data-stu-id="7ce66-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="7ce66-105">Въз основа на обратна връзка от клиенти, ние вече няма да позволяваме на правилата за имейл поток на Exchange автоматично да шифроват автоматично изходящ имейл, съдържащ определен тип поверителна информация във вашия клиент по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="7ce66-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="7ce66-106">Вместо това, ние предоставяме подробни инструкции как можете да го направите сами.</span><span class="sxs-lookup"><span data-stu-id="7ce66-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="7ce66-107">За допълнителна информация относно създаването на транспортно правило за шифроване на чувствителна информация [вж.](https://aka.ms/OmeEtr)</span><span class="sxs-lookup"><span data-stu-id="7ce66-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="7ce66-108">Ако използвате Outlook в уеб (преди **OWA):** Когато композирате имейл съобщение, просто щракнете върху **Защитете** в OWA.</span><span class="sxs-lookup"><span data-stu-id="7ce66-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="7ce66-109">Това ще се прилага "Не препращай" разрешение.</span><span class="sxs-lookup"><span data-stu-id="7ce66-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="7ce66-110">Щракнете върху **Промяна на разрешението** и изберете **Шифроване,** за да шифровате само съобщението.</span><span class="sxs-lookup"><span data-stu-id="7ce66-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="7ce66-111">Ако използвате **клиент на Outlook**: За да изпратите шифровано съобщение от Outlook 2013 или 2016 или Outlook 2016 за Mac, изберете **Опции**  >  **разрешения**, след което изберете опцията за защита, която ви е необходима.</span><span class="sxs-lookup"><span data-stu-id="7ce66-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="7ce66-112">За **да шифровате автоматично всички имейли,** изпратени до определени получатели или външни партньорски организации, трябва да създадете транспортно правило за пощенски поток в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ce66-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="7ce66-113">Подробни инструкции са дадени в [тази статия за поддръжка](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="7ce66-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

