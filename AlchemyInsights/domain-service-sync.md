---
title: Синхронизиране на услуги на домейни
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884843"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="8a2e1-102">Синхронизиране на услуги на домейни</span><span class="sxs-lookup"><span data-stu-id="8a2e1-102">Domain service synchronization</span></span>

<span data-ttu-id="8a2e1-103">За обектите и идентификационните данни в Azure Active Directory Domain Services (Azure AD DS) управляван домейн може да бъде създаден локално в домейна или синхронизиран от клиент на Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="8a2e1-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="8a2e1-104">Когато за първи път разположите Azure AD DS, автоматично се конфигурира еднопосочно синхронизиране, за да се копират обектите от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a2e1-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="8a2e1-105">Тази еднопосочна синхронизация продължава да работи във фонов режим, за да се поддържа Сайтът за управление на Azure AD DS актуализиран с всякакви промени от Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a2e1-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="8a2e1-106">Не се извършва синхронизиране от Azure AD DS обратно в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8a2e1-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="8a2e1-107">За повече информация относно синхронизацията на услугата Azure Active Directory, вижте [Синхронизиране на услугата за домейни](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="8a2e1-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
