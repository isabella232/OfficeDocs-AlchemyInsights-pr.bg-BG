---
title: Изпратете имейл съобщение, като предоставите ИД на мрежовото съобщение
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692599"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="d0b0e-102">Изпратете имейл съобщение, като предоставите ИД на мрежовото съобщение</span><span class="sxs-lookup"><span data-stu-id="d0b0e-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="d0b0e-103">В изплаващо за **нови подавания** изберете **имейл** и **мрежово съобщение ИД**.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="d0b0e-104">Следвайте тези стъпки, за да намерите ИД на съобщението за имейл съобщение в Outlook:</span><span class="sxs-lookup"><span data-stu-id="d0b0e-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="d0b0e-105">Щракнете двукратно върху имейл съобщението, за да го отворите.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="d0b0e-106">Изберете   >  **свойствата** на файла.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="d0b0e-107">Отворете Notepad или празен документ на Word и след това копирайте и поставете съдържанието, намерено в полето **интернет заглавки** , в отворения документ за по-добра видимост.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="d0b0e-108">Намерете **X-MS-Exchange-организация-мрежа-съобщение-ИД** на поле.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="d0b0e-109">Стойността след **:** представлява ли желаният от вас ИД за вашата заявка.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="d0b0e-110">Под **получатели**, ако имейлът е разтоварен в папката "нежелана поща" за всички получатели на този имейл, изберете **Избери всички**.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="d0b0e-111">Ако не е, изберете само потребителя, който е съобщил за проблема.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="d0b0e-112">Под **причина за подаване**, ако изберете **трябва да бъде блокиран**, укажете дали съобщението трябва да е блокирано като **нежелана поща**, **фишинг** или **злонамерен софтуер**, и след това изберете **Подай**.</span><span class="sxs-lookup"><span data-stu-id="d0b0e-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="d0b0e-113">За да научите повече, вижте [как да подадете предполагаем спам, Фиш, URL адреси и файлове към Microsoft за сканиране](https://go.microsoft.com/fwlink/?linkid=2101479).</span><span class="sxs-lookup"><span data-stu-id="d0b0e-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
