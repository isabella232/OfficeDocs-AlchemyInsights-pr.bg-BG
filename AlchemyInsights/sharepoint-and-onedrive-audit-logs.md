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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068012"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="81997-102">Регистрационни файлове за проверка на SharePoint и OneDrive</span><span class="sxs-lookup"><span data-stu-id="81997-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="81997-103">**SharePoint и OneDrive съвременни единни проверка регистрационни файлове от съответствие**</span><span class="sxs-lookup"><span data-stu-id="81997-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="81997-104">Включване/изключване на единно регистриране на проверка</span><span class="sxs-lookup"><span data-stu-id="81997-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="81997-105">Не се изисква допълнителна конфигурация в SharePoint или OneDrive.</span><span class="sxs-lookup"><span data-stu-id="81997-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="81997-106">Използвайте проверка регистриране на търсене, за да проверите активността на файлове, папки, потребител (и), разрешения:</span><span class="sxs-lookup"><span data-stu-id="81997-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="81997-107">Дейности с файлове и страници</span><span class="sxs-lookup"><span data-stu-id="81997-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="81997-108">Дейности в папките</span><span class="sxs-lookup"><span data-stu-id="81997-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="81997-109">Споделяне и достъп до дейности по заявка</span><span class="sxs-lookup"><span data-stu-id="81997-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="81997-110">Дейности по синхронизация</span><span class="sxs-lookup"><span data-stu-id="81997-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="81997-111">Дейности по администриране на сайта</span><span class="sxs-lookup"><span data-stu-id="81997-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="81997-112">За повече информация как да извлечете тези събития вижте [търсене в регистрационния файл на проверката](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="81997-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="81997-113">**Регистрационни файлове на SharePoint класически проверка**</span><span class="sxs-lookup"><span data-stu-id="81997-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="81997-114">Ние мигрират спо наследени проверка на единни проверка регистрационен файл.</span><span class="sxs-lookup"><span data-stu-id="81997-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="81997-115">По същество това означава, че всички съществуващи доклади за одит на спо ще бъдат захранвани чрез програмата за проверка на данни, а стари одитни сигнали са мигрирали към него.</span><span class="sxs-lookup"><span data-stu-id="81997-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="81997-116">Основни промени:</span><span class="sxs-lookup"><span data-stu-id="81997-116">Key changes:</span></span>

- <span data-ttu-id="81997-117">Почистването като възможност не е налично.</span><span class="sxs-lookup"><span data-stu-id="81997-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="81997-118">Разделът, в който избирате конкретни събития за проверка, не е наличен.</span><span class="sxs-lookup"><span data-stu-id="81997-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="81997-119">Моля, вижте [този документ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) за пълен списък на одитираните събития, налични по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="81997-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="81997-120">Опцията "местоположение" под **персонализирани отчети** не е налична.</span><span class="sxs-lookup"><span data-stu-id="81997-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="81997-121">"Отваряне или изтегляне на документи" събития не е налична.</span><span class="sxs-lookup"><span data-stu-id="81997-121">“Opening or downloading documents” events is NOT available.</span></span> 

