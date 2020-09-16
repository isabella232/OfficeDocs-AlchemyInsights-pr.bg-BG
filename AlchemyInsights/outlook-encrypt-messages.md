---
title: S/MIME в Outlook в уеб
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772251"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="cb966-102">Шифроване на имейл съобщения в Outlook</span><span class="sxs-lookup"><span data-stu-id="cb966-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="cb966-103">Шифроването на съобщения в Microsoft 365 е вградено в Microsoft Azure Rights Management (Azure RMS), който е част от защитата на Azure Information.</span><span class="sxs-lookup"><span data-stu-id="cb966-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="cb966-104">Ако абонаментът ви включва Azure Rights Management или Azure Information Protection, не **е нужно да правите нищо, за да разрешите ръчно или да активирате** услугата за управление на правата.</span><span class="sxs-lookup"><span data-stu-id="cb966-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="cb966-105">Въз основа на обратната връзка от клиентите, ние вече няма да разрешаваме правилата за пощенския поток, за да Шифроваме автоматично изходящи имейли, които съдържат определен тип поверителна информация в своя клиент по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="cb966-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="cb966-106">Вместо това ще ви предоставим подробни инструкции как да направите това сами.</span><span class="sxs-lookup"><span data-stu-id="cb966-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="cb966-107">За допълнителна информация как да създадете транспортно правило за шифроване на поверителна информация вижте [тази статия](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="cb966-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="cb966-108">Ако използвате Outlook в уеб (наричан преди **OWA**): Когато съставяте имейл съобщение, просто щракнете върху **защита** в OWA.</span><span class="sxs-lookup"><span data-stu-id="cb966-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="cb966-109">Това ще приложи разрешение "не Препращай".</span><span class="sxs-lookup"><span data-stu-id="cb966-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="cb966-110">Щракнете върху **Промяна на разрешенията** и изберете **шифроване** , за да шифровате само съобщението.</span><span class="sxs-lookup"><span data-stu-id="cb966-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="cb966-111">Ако използвате **клиент на Outlook**: за да изпратите шифровано съобщение от Outlook 2013 или 2016 или Outlook 2016 for Mac, изберете разрешения за **Опции**  >  **Permissions**, след което изберете опцията за защита, която ви е необходима.</span><span class="sxs-lookup"><span data-stu-id="cb966-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="cb966-112">За да **шифровате автоматично всички имейли** , изпратени до определени получатели или външни партньорски организации, трябва да създадете правило за транспортен поток за пощенските съобщения в центъра за администриране на Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb966-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="cb966-113">Подробни инструкции се предоставят в [тази статия от поддръжката](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="cb966-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

