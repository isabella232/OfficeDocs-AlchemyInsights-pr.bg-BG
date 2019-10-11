---
title: Заседнала в изходяща кутия поради големи прикачени файлове
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441295"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="acd6d-102">Поправяне на съобщения, които са блокирани в папката "Изходящи"</span><span class="sxs-lookup"><span data-stu-id="acd6d-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="acd6d-103">Препоръчваме ви да започнете, като изпълните сценария ["имам проблеми при изпращане, получаване или намиране на имейл съобщения"](https://aka.ms/SaRA-OutlookSendReceive) от инструмента за [поддръжка на Microsoft и помощник за възстановяване](https://diagnostics.office.com/#/) .</span><span class="sxs-lookup"><span data-stu-id="acd6d-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="acd6d-104">Когато съобщение се заби в папката "Изходящи", най-вероятните причини са:</span><span class="sxs-lookup"><span data-stu-id="acd6d-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="acd6d-105">Големи прикачени файлове.</span><span class="sxs-lookup"><span data-stu-id="acd6d-105">Large attachments.</span></span>
- <span data-ttu-id="acd6d-106">**Изпращане незабавно, когато връзката** опция не е разрешена.</span><span class="sxs-lookup"><span data-stu-id="acd6d-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="acd6d-107">За да премахнете големи прикачени файлове:</span><span class="sxs-lookup"><span data-stu-id="acd6d-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="acd6d-108">В Outlook изберете **Изпращане/получаване** > на**работа офлайн**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="acd6d-109">В навигационния екран изберете **изходяща поща**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="acd6d-110">От тук можете да:</span><span class="sxs-lookup"><span data-stu-id="acd6d-110">From here, you can:</span></span> 
    - <span data-ttu-id="acd6d-111">Изтрийте съобщението (изберете го и след това изберете **Изтрий**).</span><span class="sxs-lookup"><span data-stu-id="acd6d-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="acd6d-112">Плъзнете съобщението в папката "Чернови", щракнете двукратно, за да го отворите, и премахнете прикачения файл, след което изберете " **Изтрий**".</span><span class="sxs-lookup"><span data-stu-id="acd6d-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="acd6d-113">Ако получите грешка, която казва, че Outlook се опитва да предаде съобщението, затворете Outlook.</span><span class="sxs-lookup"><span data-stu-id="acd6d-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="acd6d-114">Може да отнеме няколко минути, за да излезете.</span><span class="sxs-lookup"><span data-stu-id="acd6d-114">It may take a few moments to exit.</span></span> <span data-ttu-id="acd6d-115">Ако Outlook не се затвори, натиснете CTRL + ALT + DELETE и изберете **Стартирай диспечера на задачите**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="acd6d-116">В диспечера на задачите изберете раздела **процеси** , превъртете надолу до Outlook. exe и изберете край на **процеса**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="acd6d-117">След като Outlook се затвори, рестартирайте го и повторете стъпки 2 и 3.</span><span class="sxs-lookup"><span data-stu-id="acd6d-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="acd6d-118">След като премахнете прикачения файл, щракнете върху **Изпращане/получаване** > на**работа офлайн** , за да възобновите работа онлайн.</span><span class="sxs-lookup"><span data-stu-id="acd6d-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="acd6d-119">Съобщенията също се залепили в кутията "Изходящи", когато щракнете върху " **Изпрати**", но не сте свързани.</span><span class="sxs-lookup"><span data-stu-id="acd6d-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="acd6d-120">Кликнете върху **Изпращане/получаване** и погледнете бутона **работа офлайн** .</span><span class="sxs-lookup"><span data-stu-id="acd6d-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="acd6d-121">Ако е синьо, ти си изключен.</span><span class="sxs-lookup"><span data-stu-id="acd6d-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="acd6d-122">Изберете го, за да се свържете (бутонът става бял) и кликнете върху **Изпращане на всички**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="acd6d-123">За да разрешите **изпращането незабавно, когато е свързано**:</span><span class="sxs-lookup"><span data-stu-id="acd6d-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="acd6d-124">Изберете \*\*\*\* > **Опции за** >  файлове**Разширени**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="acd6d-125">В секцията **Изпращане и получаване** изберете **Изпращане веднага, когато е свързано**, и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="acd6d-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="acd6d-126">За пълни подробности вижте:</span><span class="sxs-lookup"><span data-stu-id="acd6d-126">For full details see:</span></span>
- [<span data-ttu-id="acd6d-127">Видео: изпращане или изтриване на блокиран имейл</span><span class="sxs-lookup"><span data-stu-id="acd6d-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="acd6d-128">Имейл остава в папката "Изходящи", докато не започнете ръчно изпращане/получаване на операция в Outlook</span><span class="sxs-lookup"><span data-stu-id="acd6d-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
