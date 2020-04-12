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
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232619"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="bbe1c-102">Коригиране на съобщенията, които са блокирани в кутията "Изходящи"</span><span class="sxs-lookup"><span data-stu-id="bbe1c-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="bbe1c-103">Препоръчваме да започнете, като стартирате сценария ["Имам проблеми при изпращане, получаване или намиране на имейл съобщения"](https://aka.ms/SaRA-OutlookSendReceive) от инструмента за поддръжка на [Microsoft и възстановяване на помощника](https://diagnostics.office.com/#/) на засегнатия компютър.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="bbe1c-104">Когато съобщението заседне в кутията "Изходящи", най-вероятната причина е голям прикачен файл или опцията "Изпращане веднага при свързване" не е разрешена.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="bbe1c-105">**Премахване на големия прикачен файл**</span><span class="sxs-lookup"><span data-stu-id="bbe1c-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="bbe1c-106">Щракнете върху **Изпращане/получаване** > **на работа офлайн**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="bbe1c-107">В навигационния екран щракнете върху **Изходящи .**</span><span class="sxs-lookup"><span data-stu-id="bbe1c-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="bbe1c-108">От тук можете да:</span><span class="sxs-lookup"><span data-stu-id="bbe1c-108">From here, you can:</span></span> 
    - <span data-ttu-id="bbe1c-109">Изтрийте съобщението.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-109">Delete the message.</span></span> <span data-ttu-id="bbe1c-110">Просто го изберете и щракнете върху **Изтрий**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="bbe1c-111">Плъзнете съобщението в папката си **за чернови**, щракнете двукратно, за да отворите съобщението, и изтрийте прикачения файл (щракнете върху него и щракнете върху **Изтрий**).</span><span class="sxs-lookup"><span data-stu-id="bbe1c-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="bbe1c-112">Ако грешка ви казва Outlook се опитва да предаде съобщението, затворете Outlook.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="bbe1c-113">Може да отнеме няколко минути да излезе.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-113">It may take a few moments to exit.</span></span> <span data-ttu-id="bbe1c-114">Ако Outlook не се затвори, натиснете **Ctrl + Alt + Delete** и щракнете върху Старт на **диспечера на задачите**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="bbe1c-115">В Диспечера на задачите изберете раздела **Процеси,** превъртете надолу до outlook.exe и щракнете върху **Край на процеса**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="bbe1c-116">След като Outlook се затвори, рестартирайте Outlook и повторете стъпки 2-3.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="bbe1c-117">След като премахнете прикачения файл, щракнете върху **Изпрати / Получаване** > **на работа офлайн,** за да премахнете избора на бутона и да продължите да работите онлайн.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="bbe1c-118">Съобщенията също така се засядат в кутията "Изходящи", когато щракнете върху **Изпрати**, но не сте свързани.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="bbe1c-119">Щракнете **върху Изпращане / получаване** и вижте бутона Работа **офлайн.**</span><span class="sxs-lookup"><span data-stu-id="bbe1c-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="bbe1c-120">Ако е синьо, връзката не е в ред.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="bbe1c-121">Щракнете върху него, за да се свържете (бутонът става бял) и щракнете върху **Изпрати всички**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="bbe1c-122">**Разрешаване на изпращане веднага при свързване**</span><span class="sxs-lookup"><span data-stu-id="bbe1c-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="bbe1c-123">В раздела файл щракнете върху **Опции**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="bbe1c-124">В диалоговия прозорец Опции на Outlook щракнете върху **Разширени**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="bbe1c-125">В раздела Изпращане и получаване щракнете, за да активирате **Изпращане веднага, когато е свързано**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="bbe1c-126">Щракнете върху **OK**.</span><span class="sxs-lookup"><span data-stu-id="bbe1c-126">Click **OK**.</span></span>
 
<span data-ttu-id="bbe1c-127">За подробности вижте:</span><span class="sxs-lookup"><span data-stu-id="bbe1c-127">For full details, see:</span></span>
- [<span data-ttu-id="bbe1c-128">Видео: Изпращане или изтриване на блокиран имейл</span><span class="sxs-lookup"><span data-stu-id="bbe1c-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="bbe1c-129">Имейл остава в папката "Изходящи", докато не стартирате ръчно операция за изпращане / получаване в Outlook</span><span class="sxs-lookup"><span data-stu-id="bbe1c-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
