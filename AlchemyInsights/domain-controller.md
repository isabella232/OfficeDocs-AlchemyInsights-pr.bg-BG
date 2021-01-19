---
title: Домейнов контролер
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900762"
---
# <a name="domain-controller"></a><span data-ttu-id="42421-102">Домейнов контролер</span><span class="sxs-lookup"><span data-stu-id="42421-102">Domain controller</span></span>

<span data-ttu-id="42421-103">**Не можете да разрешите използването на пад-DS или разполагане е неуспешно**</span><span class="sxs-lookup"><span data-stu-id="42421-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="42421-104">За да се реши проблемът с услугата за домейни на Azure AD (пад-DS), която не е разрешена или не може да бъде разгърната, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="42421-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="42421-105">Ако използвате вече съществуваща виртуална мрежа, проверете своя ГЯД за правила, които блокират портове, необходими за синхронизиране в пад-DS в портала https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="42421-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="42421-106">Проверете дали за съобщението за грешка е отговорено в това ръководство за отстраняване на неизправности, което е налично в  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="42421-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="42421-107">Опитайте да разположите услугите за домейни на Azure AD в нова виртуална мрежа.</span><span class="sxs-lookup"><span data-stu-id="42421-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="42421-108">Следвайте ръководството "Начално запознаване" как да разположите пад-DS, което е налично в [ръководството, за да създадете AZURE ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="42421-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="42421-109">Ако имате проблеми с разполагането на Azure AD Domain Services, вижте [отстраняване на неизправности в AZURE ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) за разрешаване на често срещани грешки, които да ви помогнат да работите отново.</span><span class="sxs-lookup"><span data-stu-id="42421-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="42421-110">**Не можете да забраните пад-DS**</span><span class="sxs-lookup"><span data-stu-id="42421-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="42421-111">ПАД-ДС не може да бъде спрян.</span><span class="sxs-lookup"><span data-stu-id="42421-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="42421-112">Ако искате да спрете да използвате своя управляван домейн, той трябва да бъде изтрит.</span><span class="sxs-lookup"><span data-stu-id="42421-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="42421-113">Ако срещнете проблеми, за да решите често срещани съобщения за грешка и за свързани стъпки за отстраняване на неизправности, за да ви помогнат да започнете да работите отново, вижте [отстраняване на неизправности в Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="42421-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
