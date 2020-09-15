---
title: Определяне на външни препращане на имейли в регистри за проверка
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696286"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="e606d-102">Определяне кога е конфигурирано външно препращане на имейл в пощенските кутии</span><span class="sxs-lookup"><span data-stu-id="e606d-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="e606d-103">Когато потребител на Microsoft 365 конфигурира външни препращане на имейли в пощенска кутия, дейността се проверява като част от кратката команда **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="e606d-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="e606d-104">Можете да видите дейността с помощта на търсене в регистрационния файл за проверка в центъра за съответствие на & за защита.</span><span class="sxs-lookup"><span data-stu-id="e606d-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="e606d-105">Влезте в центъра за [съответствие на & на Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e606d-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e606d-106">Отидете на страницата **Search**за  >  **търсене в регистрационния файл за проверка** на търсенето.</span><span class="sxs-lookup"><span data-stu-id="e606d-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="e606d-107">Изберете диапазона от дати в полетата " **Начална дата** " и " **крайна дата** ".</span><span class="sxs-lookup"><span data-stu-id="e606d-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="e606d-108">Не е нужно да указвате потребителско име.</span><span class="sxs-lookup"><span data-stu-id="e606d-108">You don't need to specify a username.</span></span> <span data-ttu-id="e606d-109">Проверете дали полето **дейности** е зададено да **показва резултати за всички дейности**.</span><span class="sxs-lookup"><span data-stu-id="e606d-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="e606d-110">Щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="e606d-110">Click **Search**.</span></span>

<span data-ttu-id="e606d-111">В резултатите щракнете върху **филтриране на резултати** и въвеждане на **набор от пощенски кутии** в полето Филтър за дейност.</span><span class="sxs-lookup"><span data-stu-id="e606d-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="e606d-112">Изберете запис за проверка в резултатите.</span><span class="sxs-lookup"><span data-stu-id="e606d-112">Select an audit record in the results.</span></span> <span data-ttu-id="e606d-113">В изплаващо за **подробни данни** щракнете върху **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="e606d-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="e606d-114">Трябва да прегледате подробностите за всеки одитен запис, за да определите дали дейността е свързана с препращане на имейли.</span><span class="sxs-lookup"><span data-stu-id="e606d-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="e606d-115">**ObjectId**: стойността за псевдоним на пощенската кутия, която е променена.</span><span class="sxs-lookup"><span data-stu-id="e606d-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="e606d-116">**Параметри**: _ForwardingSmtpAddress_ указва целевия имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="e606d-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="e606d-117">**Потребителско име**: потребителя, който е конфигурирал препращане на имейл в пощенската кутия в полето **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="e606d-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="e606d-118">За повече информация вижте [определяне кой е настроил препращане на имейл за пощенска кутия](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="e606d-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
