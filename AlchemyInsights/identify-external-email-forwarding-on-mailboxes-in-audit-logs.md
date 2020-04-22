---
title: Идентифициране на външни имейл препращане на пощенски кутии в регистрационните файлове за проверка
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716449"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="c049e-102">Проверете при пренасочване на външни имейл е конфигуриран на пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="c049e-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="c049e-103">Когато потребител на Microsoft 365 конфигурира външни имейл препращане на пощенска кутия, дейността се проверява като част от кратката команда **Set-пощенска кутия.**</span><span class="sxs-lookup"><span data-stu-id="c049e-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="c049e-104">Можете да видите дейността, като използвате проверка регистър търсене в центъра за съответствие на защитата &.</span><span class="sxs-lookup"><span data-stu-id="c049e-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="c049e-105">Влезте в центъра за сигурност на [Microsoft 365 & съответствие .](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="c049e-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="c049e-106">Отидете на страницата **за** > **търсене на регистрационния файл за проверка.**</span><span class="sxs-lookup"><span data-stu-id="c049e-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="c049e-107">Изберете периода от време в полетата **Начална дата** и **Крайна дата.**</span><span class="sxs-lookup"><span data-stu-id="c049e-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="c049e-108">Не е необходимо да посочвате потребителско име.</span><span class="sxs-lookup"><span data-stu-id="c049e-108">You don't need to specify a username.</span></span> <span data-ttu-id="c049e-109">Проверете дали полето **Дейности** е настроено да **Показва резултатите за всички дейности**.</span><span class="sxs-lookup"><span data-stu-id="c049e-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="c049e-110">Щракнете върху **Търсене**.</span><span class="sxs-lookup"><span data-stu-id="c049e-110">Click **Search**.</span></span>

<span data-ttu-id="c049e-111">В резултатите щракнете върху **Филтър резултати** и въведете **Set-пощенска кутия** в полето за филтър на дейност .</span><span class="sxs-lookup"><span data-stu-id="c049e-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="c049e-112">Изберете запис за проверка в резултатите.</span><span class="sxs-lookup"><span data-stu-id="c049e-112">Select an audit record in the results.</span></span> <span data-ttu-id="c049e-113">В допълнителното меню **Подробности** щракнете върху **Още информация**.</span><span class="sxs-lookup"><span data-stu-id="c049e-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="c049e-114">Трябва да разгледате подробностите за всеки запис за проверка, за да определите дали дейността е свързана с препращане на имейл.</span><span class="sxs-lookup"><span data-stu-id="c049e-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="c049e-115">**ObjectId**: Ид на псевдоним на пощенскакутия, която е модифицирана.</span><span class="sxs-lookup"><span data-stu-id="c049e-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="c049e-116">**Параметри:** _ForwardingSmtpAddress_ показва целевия имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="c049e-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="c049e-117">**UserId:** Потребителят, който е конфигурирал препращане на имейл на пощенската кутия в полето **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="c049e-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="c049e-118">За повече информация вижте [Определяне кой да настроите имейл препращане за пощенска кутия](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c049e-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
