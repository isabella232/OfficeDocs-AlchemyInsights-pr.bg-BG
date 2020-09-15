---
title: Класически отчети на регистрационни файлове за проверка на SharePoint
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662197"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="6345f-102">Регистрационни файлове за проверка на SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="6345f-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="6345f-103">Регистрационни файлове за проверка на класическия SharePoint</span><span class="sxs-lookup"><span data-stu-id="6345f-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="6345f-104">За да бъде мигриран Архивът за един и същ регистър за проверка (изп).</span><span class="sxs-lookup"><span data-stu-id="6345f-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="6345f-105">Всички наследени отчети за проверка на всички данни ще се захранват чрез изп и наследените сигнали за проверка са мигрирани към изп.</span><span class="sxs-lookup"><span data-stu-id="6345f-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="6345f-106">Клавишни промени:</span><span class="sxs-lookup"><span data-stu-id="6345f-106">Key changes:</span></span>

* <span data-ttu-id="6345f-107">Изрязването не е достъпно като способност.</span><span class="sxs-lookup"><span data-stu-id="6345f-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="6345f-108">Избирането на конкретни събития за проверка не е налично.</span><span class="sxs-lookup"><span data-stu-id="6345f-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="6345f-109">Вижте [този документ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, които са налични по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="6345f-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="6345f-110">Опцията за **местоположение** под **персонализирани отчети** е недостъпна.</span><span class="sxs-lookup"><span data-stu-id="6345f-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="6345f-111">Опцията за **Отваряне или изтегляне на документи** е недостъпна.</span><span class="sxs-lookup"><span data-stu-id="6345f-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="6345f-112">Конфигуриране на настройки за проверка на колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="6345f-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="6345f-113">Нови регистри за унифицирани проверки на SharePoint и OneDrive за съответствие</span><span class="sxs-lookup"><span data-stu-id="6345f-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="6345f-114">Включване/изключване на регистрирането на унифицирани проверки</span><span class="sxs-lookup"><span data-stu-id="6345f-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="6345f-115">Не се изисква допълнителна конфигурация в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6345f-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="6345f-116">Използване на търсене в регистрационния файл за проверка, за да се провери дейността на файловете, папките, потребителите, разрешенията:</span><span class="sxs-lookup"><span data-stu-id="6345f-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="6345f-117">Дейности с файлове и страници</span><span class="sxs-lookup"><span data-stu-id="6345f-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="6345f-118">Дейности с папки</span><span class="sxs-lookup"><span data-stu-id="6345f-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="6345f-119">Дейности за споделяне и достъп до заявка</span><span class="sxs-lookup"><span data-stu-id="6345f-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="6345f-120">Дейности за синхронизиране</span><span class="sxs-lookup"><span data-stu-id="6345f-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="6345f-121">Дейности за администриране на сайт</span><span class="sxs-lookup"><span data-stu-id="6345f-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="6345f-122">За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл за проверка](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="6345f-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
