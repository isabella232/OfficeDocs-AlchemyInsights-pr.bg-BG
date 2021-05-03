---
title: Проблеми с SharePoint на Windows 7 машини
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124815"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="02964-102">Проблеми с SharePoint на Windows 7 машини</span><span class="sxs-lookup"><span data-stu-id="02964-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="02964-103">Ако получите грешки на Windows 7 машини, докато работите на SharePoint или OneDrive, те може да са свързани с отстраняването на TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="02964-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="02964-104">За повече информация вижте:</span><span class="sxs-lookup"><span data-stu-id="02964-104">For more information, see:</span></span>

- [<span data-ttu-id="02964-105">Подготовка за TLS 1,2 в Office 365 и Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="02964-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="02964-106">Windows 7 SP1/Windows 8 трябва да имат разрешен TLS1.2.</span><span class="sxs-lookup"><span data-stu-id="02964-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="02964-107">За повече информация вижте Грешки [при удостоверяване възникват, когато клиентът няма поддръжка на TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="02964-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="02964-108">Инсталирайте KB3140245 и създайте стойността в системния регистър.</span><span class="sxs-lookup"><span data-stu-id="02964-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="02964-109">За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) като защитени протоколи по подразбиране в WinHTTP в Windows</span><span class="sxs-lookup"><span data-stu-id="02964-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="02964-110">Windows 7 SP1/Windows 8 трябва да гарантират, че са инсталирани най-новите пакети за шифроване на TLS.</span><span class="sxs-lookup"><span data-stu-id="02964-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="02964-111">За повече информация вижте [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="02964-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


