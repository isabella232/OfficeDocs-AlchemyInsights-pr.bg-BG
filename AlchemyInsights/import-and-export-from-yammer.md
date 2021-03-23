---
title: Импортиране и експортиране от Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034918"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="315b7-102">Импортиране и експортиране от Yammer</span><span class="sxs-lookup"><span data-stu-id="315b7-102">Import and export from Yammer</span></span>

<span data-ttu-id="315b7-103">**Импортиране**</span><span class="sxs-lookup"><span data-stu-id="315b7-103">**Import**</span></span>

<span data-ttu-id="315b7-104">Опциите за импортиране на потребители са различни в зависимост от това дали вашата мрежа на Yammer е в [основен режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), или не.</span><span class="sxs-lookup"><span data-stu-id="315b7-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="315b7-105">**Non-Native режим**: потребителите могат да бъдат импортирани в групи с помощта на " [Добавяне от адресната книга](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) " (лимит към потребители на 100) в настройките на група или в мрежата чрез [групово актуализиране](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в Network Admin.</span><span class="sxs-lookup"><span data-stu-id="315b7-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="315b7-106">**Native Mode**: членството в група и операцията за членство в мрежата трябва да се извършва от [портала за администриране на Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [портала на Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)или чрез друга опция за Azure ad.</span><span class="sxs-lookup"><span data-stu-id="315b7-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="315b7-107">Мрежите в основен режим вече нямат достъп до групово актуализиране и други наследени функции.</span><span class="sxs-lookup"><span data-stu-id="315b7-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="315b7-108">Yammer никога не поддържа импортиране на съдържание в рамките на мрежата, дори когато функцията за експортиране на данни е използвана в друга мрежа.</span><span class="sxs-lookup"><span data-stu-id="315b7-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="315b7-109">Съдържанието може да бъде повторно Публикувано от партньорски решения или API за почивка на Yammer.</span><span class="sxs-lookup"><span data-stu-id="315b7-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="315b7-110">**Експортиране**</span><span class="sxs-lookup"><span data-stu-id="315b7-110">**Export**</span></span>

<span data-ttu-id="315b7-111">[Експортирането на данни на мрежата в мрежата](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) позволява експортирането на съдържание от мрежите на Yammer, включително съобщенията и файловете.</span><span class="sxs-lookup"><span data-stu-id="315b7-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="315b7-112">Прикачените файлове могат да бъдат изключително големи и ще предизвикат износа, за да се извърши значителен период от време.</span><span class="sxs-lookup"><span data-stu-id="315b7-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="315b7-113">Препоръчваме активните мрежи да се експортират посредством [API за експортиране на данни](https://developer.yammer.com/docs/data-export-api) на части по ден или седмица.</span><span class="sxs-lookup"><span data-stu-id="315b7-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="315b7-114">Поддръжката на Microsoft не предоставя скриптове по избор за тази цел.</span><span class="sxs-lookup"><span data-stu-id="315b7-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="315b7-115">Съществува отделен [GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) за експортиране, за да се експортира съдържание за отделен потребител.</span><span class="sxs-lookup"><span data-stu-id="315b7-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>