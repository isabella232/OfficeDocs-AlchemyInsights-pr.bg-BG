---
title: Идентифицира външни имейл изпращане на пощенски кутии в регистрационните файлове от одита
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751982"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="b4104-102">Идентифициране при външни имейл препращане е конфигуриран на пощенски кутии</span><span class="sxs-lookup"><span data-stu-id="b4104-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="b4104-103">Когато даден потребител конфигурира външни имейл препращане на пощенска кутия, дейността е одит като част от кратката команда **Set -** Mailbox.</span><span class="sxs-lookup"><span data-stu-id="b4104-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="b4104-104">Можете да видите дейността чрез одит регистрационния файл търсене в защита & съответствие център.</span><span class="sxs-lookup"><span data-stu-id="b4104-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="b4104-105">Влезте в [Office 365 сигурност & съответствие център](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b4104-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b4104-106">Щракнете върху **търсене и проучване** и изберете **Одит регистрационния файл търсене**.</span><span class="sxs-lookup"><span data-stu-id="b4104-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b4104-107">Изберете диапазона от дати в полетата **Начална дата** и **крайна дата** .</span><span class="sxs-lookup"><span data-stu-id="b4104-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b4104-108">Не е нужно да укажете потребителско име.</span><span class="sxs-lookup"><span data-stu-id="b4104-108">You don't need to specify a username.</span></span> <span data-ttu-id="b4104-109">Проверете полето **дейности** е зададена да **покаже резултати за всички дейности**.</span><span class="sxs-lookup"><span data-stu-id="b4104-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="b4104-110">Щракнете върху **търсене**.</span><span class="sxs-lookup"><span data-stu-id="b4104-110">Click **Search**.</span></span>

<span data-ttu-id="b4104-111">В резултатите щракнете върху **Филтър резултатите** и въведете **Set-пощенска кутия** в полето на филтъра дейност.</span><span class="sxs-lookup"><span data-stu-id="b4104-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="b4104-112">Изберете отчет в резултатите.</span><span class="sxs-lookup"><span data-stu-id="b4104-112">Select an audit record in the results.</span></span> <span data-ttu-id="b4104-113">В **детайли** flyout щракнете върху **повече информация**.</span><span class="sxs-lookup"><span data-stu-id="b4104-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="b4104-114">Вие трябва да погледнете в детайлите на всеки одит запис да се определи дали дейността е свързана с имейл препращане.</span><span class="sxs-lookup"><span data-stu-id="b4104-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="b4104-115">**ObjectId**: псевдоним стойността на пощенска кутия, която е модифициран.</span><span class="sxs-lookup"><span data-stu-id="b4104-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="b4104-116">**Параметри**: _ForwardingSmtpAddress_ показва на целеви имейл адрес.</span><span class="sxs-lookup"><span data-stu-id="b4104-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="b4104-117">**Потребителско име**: потребител, който е конфигуриран имейл препращане на пощенската кутия в полето **ObjectId** .</span><span class="sxs-lookup"><span data-stu-id="b4104-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="b4104-118">За повече информация вижте [определя кой създаде имейл спедиция за пощенска кутия](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="b4104-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
