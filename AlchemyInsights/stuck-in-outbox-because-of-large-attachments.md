---
title: Блокирани в изходящи тела поради големи прикачени файлове
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
- "9002385"
- "4645"
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241241"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="bbbb4-102">Коригиране на съобщенията, които са блокирани в кутията "Изходящи"</span><span class="sxs-lookup"><span data-stu-id="bbbb4-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="bbbb4-103">Препоръчваме да започнете, като стартирате сценария ["Имам проблеми при изпращане, получаване или намиране на имейл съобщения"](https://aka.ms/SaRA-OutlookSendReceive) от инструмента [за поддръжка на Microsoft и възстановяване на помощника.](https://diagnostics.office.com/#/)</span><span class="sxs-lookup"><span data-stu-id="bbbb4-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="bbbb4-104">Когато съобщението заседне в кутията "Изходящи", най-вероятната причина е голям прикачен файл или опцията "Изпращане веднага при свързване" не е разрешена.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="bbbb4-105">**Премахване на големия прикачен файл**</span><span class="sxs-lookup"><span data-stu-id="bbbb4-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="bbbb4-106">В Outlook изберете **Изпращане / получаване** > **на работа офлайн**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="bbbb4-107">В навигационния екран изберете **Изходящи**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="bbbb4-108">От тук можете да:</span><span class="sxs-lookup"><span data-stu-id="bbbb4-108">From here, you can:</span></span> 
    - <span data-ttu-id="bbbb4-109">Изтрийте съобщението (изберете го и след това изберете **Изтрий**).</span><span class="sxs-lookup"><span data-stu-id="bbbb4-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="bbbb4-110">Плъзнете съобщението в папката "Чернови", щракнете двукратно, за да го отворите, и премахнете прикачения файл, след което изберете иконата на прикачен файл и след това изберете **Изтрий**).</span><span class="sxs-lookup"><span data-stu-id="bbbb4-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="bbbb4-111">Ако получите съобщение за грешка, която казва, че Outlook се опитва да предаде съобщението, затворете Outlook.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="bbbb4-112">Може да отнеме няколко минути да излезе.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-112">It may take a few moments to exit.</span></span> <span data-ttu-id="bbbb4-113">Ако Outlook не се затвори, натиснете Ctrl + Alt + Delete и изберете **Стартирай диспечера на задачите**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="bbbb4-114">В Диспечера на задачите изберете раздела **Процеси,** превъртете надолу до outlook.exe и изберете **Край на процеса**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="bbbb4-115">След като Outlook се затвори, рестартирайте го и повторете стъпки 2 и 3.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="bbbb4-116">След като премахнете прикачения файл, щракнете върху **Изпрати / Получаване** > **на работа офлайн,** за да продължите работа онлайн.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="bbbb4-117">Съобщенията също така се засядат в кутията "Изходящи", когато щракнете върху **Изпрати**, но не сте свързани.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="bbbb4-118">Щракнете **върху Изпращане / получаване** и вижте бутона Работа **офлайн.**</span><span class="sxs-lookup"><span data-stu-id="bbbb4-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="bbbb4-119">Ако е синьо, връзката не е в ред.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="bbbb4-120">Щракнете върху него, за да се свържете (бутонът става бял) и щракнете върху **Изпрати всички**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="bbbb4-121">**Разрешаване на изпращане веднага при свързване**</span><span class="sxs-lookup"><span data-stu-id="bbbb4-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="bbbb4-122">В раздела файл щракнете върху **Опции**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="bbbb4-123">В диалоговия прозорец Опции на Outlook щракнете върху **Разширени**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="bbbb4-124">В раздела Изпращане и получаване щракнете, за да активирате **Изпращане веднага, когато е свързано**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="bbbb4-125">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="bbbb4-125">Click **OK**.</span></span>
 
<span data-ttu-id="bbbb4-126">За подробности вижте:</span><span class="sxs-lookup"><span data-stu-id="bbbb4-126">For full details, see:</span></span>
- [<span data-ttu-id="bbbb4-127">Видео: Изпращане или изтриване на блокиран имейл</span><span class="sxs-lookup"><span data-stu-id="bbbb4-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="bbbb4-128">Имейл остава в папката "Изходящи", докато не стартирате ръчно операция за изпращане / получаване в Outlook</span><span class="sxs-lookup"><span data-stu-id="bbbb4-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
