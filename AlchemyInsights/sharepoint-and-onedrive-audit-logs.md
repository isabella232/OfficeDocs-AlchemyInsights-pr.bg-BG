---
title: Класически отчети на регистрационния файл за проверка на SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741954"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="f5707-102">Регистрационни файлове за проверка на SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="f5707-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="f5707-103">Класически регистрационни файлове за проверка на SharePoint</span><span class="sxs-lookup"><span data-stu-id="f5707-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="f5707-104">SPO одитът на наследството е пренесен в единни регистрационен файл за проверка (UAL).</span><span class="sxs-lookup"><span data-stu-id="f5707-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="f5707-105">Всички sPO одитни доклади сега ще бъде захранван чрез UAL и стари одит сигнали са пренесени в UAL.</span><span class="sxs-lookup"><span data-stu-id="f5707-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="f5707-106">Основни промени:</span><span class="sxs-lookup"><span data-stu-id="f5707-106">Key changes:</span></span>

* <span data-ttu-id="f5707-107">Подстригването НЕ е налично като възможност.</span><span class="sxs-lookup"><span data-stu-id="f5707-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="f5707-108">Изборът на конкретни събития за проверка НЕ е наличен.</span><span class="sxs-lookup"><span data-stu-id="f5707-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="f5707-109">Вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитирани събития, налични по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="f5707-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="f5707-110">Опцията **Местоположение** под **Персонализирани отчети** НЕ е налична.</span><span class="sxs-lookup"><span data-stu-id="f5707-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="f5707-111">Опцията **За отваряне или изтегляне на документи** събития не е налична.</span><span class="sxs-lookup"><span data-stu-id="f5707-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="f5707-112">Конфигуриране на настройките за проверка за колекция от сайтове</span><span class="sxs-lookup"><span data-stu-id="f5707-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="f5707-113">Регистрационнифайлове за проверка на SharePoint и OneDrive съвременни единни проверки от съответствието</span><span class="sxs-lookup"><span data-stu-id="f5707-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="f5707-114">Включване/изключване на регистрирането на единни одит</span><span class="sxs-lookup"><span data-stu-id="f5707-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="f5707-115">Не се изисква допълнителна конфигурация в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f5707-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="f5707-116">Използвайте проверка на регистрирането търсене, за да проверите дейността на файловете, папките, потребителите, разрешенията:</span><span class="sxs-lookup"><span data-stu-id="f5707-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="f5707-117">Дейности по файловете и страниците</span><span class="sxs-lookup"><span data-stu-id="f5707-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="f5707-118">Дейности в папки</span><span class="sxs-lookup"><span data-stu-id="f5707-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="f5707-119">Дейности за споделяне и достъп до заявки</span><span class="sxs-lookup"><span data-stu-id="f5707-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="f5707-120">Дейности по синхронизиране</span><span class="sxs-lookup"><span data-stu-id="f5707-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="f5707-121">Административни дейности на обекта</span><span class="sxs-lookup"><span data-stu-id="f5707-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="f5707-122">За повече информация как да извлечете тези събития вижте [Търсене в регистрационния файл за проверка](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="f5707-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
