---
title: Управление на глобалния адресен списък на организацията и офлайн адресната книга
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022368"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="a7e02-102">Управление на глобалния адресен списък (GAL) на организацията и офлайн адресната книга (OAB)</span><span class="sxs-lookup"><span data-stu-id="a7e02-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="a7e02-103">Глобалният адресен списък (GAL) е списък на обектите с активиран имейл (всякакъв тип получател, който може да получи имейл) в организацията.</span><span class="sxs-lookup"><span data-stu-id="a7e02-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="a7e02-104">Във всяка организация автоматично се създава един GAL.</span><span class="sxs-lookup"><span data-stu-id="a7e02-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="a7e02-105">Можете да създадете допълнителни GAL за отделни потребители по организация или местоположение, но един потребител може да вижда и използва само един GAL в даден момент.</span><span class="sxs-lookup"><span data-stu-id="a7e02-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="a7e02-106">Някои имейл клиенти, като например Outlook за Windows, изтеглят GAL за използване офлайн.</span><span class="sxs-lookup"><span data-stu-id="a7e02-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="a7e02-107">Това се нарича офлайн адресна книга (OAB).</span><span class="sxs-lookup"><span data-stu-id="a7e02-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="a7e02-108">В Exchange Online OAB се актуализира само веднъж на всеки 8 часа, а след това клиентите трябва да го изтеглят, за да актуализират своето локално копие на OAB.</span><span class="sxs-lookup"><span data-stu-id="a7e02-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="a7e02-109">Всеки получател трябва първо да се вижда в GAL, за да го направи по-късно в OAB.</span><span class="sxs-lookup"><span data-stu-id="a7e02-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="a7e02-110">Ето някои често използвани процедури за GAL и OAB:</span><span class="sxs-lookup"><span data-stu-id="a7e02-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="a7e02-111">По различни причини може да искате някои обекти да бъдат скрити от GAL.</span><span class="sxs-lookup"><span data-stu-id="a7e02-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="a7e02-112">Вж. [Скриете получателите от списъците с адреси](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="a7e02-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="a7e02-113">Ако трябва да предоставите на конкретни групи от потребители персонализирани изгледи на GAL на организацията, вж. [Правила за адресната книга в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="a7e02-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="a7e02-114">[Създайте глобален адресен списък в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) и научите как да работите с разрешения на GAL, вж. [Адресни списъци в Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="a7e02-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="a7e02-115">Обърнете внимание, че ако създадете нови GAL, може също да искате да създадете нов OAB.</span><span class="sxs-lookup"><span data-stu-id="a7e02-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="a7e02-116">Вж. [Процедурите за офлайн адресна книга](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="a7e02-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
