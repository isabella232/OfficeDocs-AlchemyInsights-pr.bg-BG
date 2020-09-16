---
title: Отстраняване на неизправности при отказан достъп
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767641"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="9410b-102">Отстраняване на проблеми с отказан достъп на съобщения в центъра за администриране на SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="9410b-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="9410b-103">Ако получавате съобщение за отказан достъп, когато се опитвате да отидете в център за администриране на SharePoint/OneDrive, се уверете, че сте [задали лиценз на потребителя](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="9410b-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="9410b-104">Ако потребителят има лиценз, трябва също да се уверите, че му е [присвоена административна роля](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , която може да получи достъп до центровете за администриране.</span><span class="sxs-lookup"><span data-stu-id="9410b-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="9410b-105">Този проблем може да възникне и когато потребителят бъде изтрит и пресъздаден със същото основно потребителско име (UPN).</span><span class="sxs-lookup"><span data-stu-id="9410b-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="9410b-106">Новият акаунт се създава с помощта на различна стойност на PUID (уникален ИД за Passport).</span><span class="sxs-lookup"><span data-stu-id="9410b-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="9410b-107">Когато потребителят се опитва да получи достъп до колекция от сайтове или техния OneDrive, потребителят има неправилни PUID.</span><span class="sxs-lookup"><span data-stu-id="9410b-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="9410b-108">Вторият сценарий включва синхронизирането на справочен указател с организационната единица за Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="9410b-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="9410b-109">Ако потребителите вече са влезли в SharePoint, а след това бъдат преместени в друга ОЕ и да се синхронизират с SharePoint, може да изпитате този проблем.</span><span class="sxs-lookup"><span data-stu-id="9410b-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="9410b-110">За да отстраните този проблем, трябва да възстановите първоначалния UPN със стъпките в статията [възстановяване на потребител в Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="9410b-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="9410b-111">Забележка: Ако един център за администриране на OneDrive или SharePoint не е достъпен за множество потребители, които преди това са имали достъп, е възможно да има временен проблем с услугата.</span><span class="sxs-lookup"><span data-stu-id="9410b-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="9410b-112">[Проверете таблото за изправност на услугите](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="9410b-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


