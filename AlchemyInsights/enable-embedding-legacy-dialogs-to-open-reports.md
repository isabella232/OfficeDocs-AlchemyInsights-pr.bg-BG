---
title: Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814253"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="f4989-102">Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети</span><span class="sxs-lookup"><span data-stu-id="f4989-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="f4989-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="f4989-103">**Symptom**</span></span>

<span data-ttu-id="f4989-104">Потребителите не могат да отварят отчети.</span><span class="sxs-lookup"><span data-stu-id="f4989-104">Users are unable to open reports.</span></span> <span data-ttu-id="f4989-105">"Нещо се обърка.</span><span class="sxs-lookup"><span data-stu-id="f4989-105">"Something has gone wrong.</span></span> <span data-ttu-id="f4989-106">Проверете техническите подробности за пояснения."</span><span class="sxs-lookup"><span data-stu-id="f4989-106">Check technical details for more details."</span></span>

<span data-ttu-id="f4989-107">**Причина**</span><span class="sxs-lookup"><span data-stu-id="f4989-107">**Cause**</span></span>

<span data-ttu-id="f4989-108">Отчетите не успяват да се заредят в UCI с грешката "Дескрипторът на формуляра е празен или не е дефиниран".</span><span class="sxs-lookup"><span data-stu-id="f4989-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="f4989-109">Отчетите в UCI все още изискват наследени диалогови прозорци, така че в системата на клиента трябва да има разрешено *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="f4989-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="f4989-110">**Решение**</span><span class="sxs-lookup"><span data-stu-id="f4989-110">**Solution**</span></span>

1. <span data-ttu-id="f4989-111">Отидете в раздела **Настройки > Администрация > Настройки на системата > Общи**.</span><span class="sxs-lookup"><span data-stu-id="f4989-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="f4989-112">Задайте "Разрешаване на вграждане на наследени диалогови прозорци за отваряне на отчети" на **Да**.</span><span class="sxs-lookup"><span data-stu-id="f4989-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
