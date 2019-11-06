---
title: Класически отчети на регистрационния файл за проверка на SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992607"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="25a79-102">Регистрационни файлове за проверка на SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="25a79-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="25a79-103">Регистрационни файлове на SharePoint класически проверка</span><span class="sxs-lookup"><span data-stu-id="25a79-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="25a79-104">СПО наследени одит е мигрирал към единни проверка регистрационен файл.</span><span class="sxs-lookup"><span data-stu-id="25a79-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="25a79-105">Всички проспо стари одиторски отчети сега ще се захранва чрез IT и стари одит сигнали са мигрирали към програмата.</span><span class="sxs-lookup"><span data-stu-id="25a79-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="25a79-106">Основни промени:</span><span class="sxs-lookup"><span data-stu-id="25a79-106">Key changes:</span></span>

* <span data-ttu-id="25a79-107">Почистването не е налично като възможност.</span><span class="sxs-lookup"><span data-stu-id="25a79-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="25a79-108">Избирането на конкретни събития за проверка не е налично.</span><span class="sxs-lookup"><span data-stu-id="25a79-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="25a79-109">Вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, налични по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="25a79-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="25a79-110">Опцията за **местоположение** под **персонализирани отчети** не е налична.</span><span class="sxs-lookup"><span data-stu-id="25a79-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="25a79-111">Опцията за **Отваряне или изтегляне на документи** събития не е налична.</span><span class="sxs-lookup"><span data-stu-id="25a79-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="25a79-112">Конфигуриране на настройките за проверка за колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="25a79-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="25a79-113">SharePoint и OneDrive съвременни единни проверка регистрационни файлове от съответствие</span><span class="sxs-lookup"><span data-stu-id="25a79-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="25a79-114">Включване/изключване на единно регистриране на проверка</span><span class="sxs-lookup"><span data-stu-id="25a79-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="25a79-115">Не се изисква допълнителна конфигурация в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="25a79-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="25a79-116">Използвайте проверка регистриране на търсене, за да проверите активността на файлове, папки, потребител (и), разрешения:</span><span class="sxs-lookup"><span data-stu-id="25a79-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="25a79-117">Дейности с файлове и страници</span><span class="sxs-lookup"><span data-stu-id="25a79-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="25a79-118">Дейности в папките</span><span class="sxs-lookup"><span data-stu-id="25a79-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="25a79-119">Споделяне и достъп до дейности по заявка</span><span class="sxs-lookup"><span data-stu-id="25a79-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="25a79-120">Дейности по синхронизация</span><span class="sxs-lookup"><span data-stu-id="25a79-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="25a79-121">Дейности по администриране на сайта</span><span class="sxs-lookup"><span data-stu-id="25a79-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="25a79-122">За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл на проверката](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="25a79-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
