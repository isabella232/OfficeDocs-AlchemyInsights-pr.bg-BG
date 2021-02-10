---
title: Проблем със защитни групи
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177367"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="d8877-102">Проблем със защитни групи</span><span class="sxs-lookup"><span data-stu-id="d8877-102">Issue with security groups</span></span>

<span data-ttu-id="d8877-103">**Ако получавате съобщение за грешка в мрежата AADDS104**</span><span class="sxs-lookup"><span data-stu-id="d8877-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="d8877-104">Невалидни правила за мрежова защита са най-честата причина за грешки в мрежата за Domain Services Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="d8877-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="d8877-105">Групата за мрежова защита за виртуалната мрежа трябва да позволява достъп до определени портове и протоколи.</span><span class="sxs-lookup"><span data-stu-id="d8877-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="d8877-106">Ако тези портове са блокирани, платформата Azure не може да следи или актуализира управлявания домейн.</span><span class="sxs-lookup"><span data-stu-id="d8877-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="d8877-107">Синхронизацията между Azure AD и Azure AD DS също е повлияна.</span><span class="sxs-lookup"><span data-stu-id="d8877-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="d8877-108">Уверете се, че сте отворили портовете по подразбиране, за да избегнете прекъсване на услугата.</span><span class="sxs-lookup"><span data-stu-id="d8877-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="d8877-109">За да разберете и да коригирате често срещани предупреждения за проблеми с конфигурацията на мрежата за мрежова защита, вижте [Добавяне и проверка на групи за защита](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="d8877-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
