---
title: Разрешаване на вграждането на наследени диалози за отваряне на отчети
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204649"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="a2d0c-102">Разрешаване на вграждането на наследени диалози за отваряне на отчети</span><span class="sxs-lookup"><span data-stu-id="a2d0c-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="a2d0c-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="a2d0c-103">**Symptom**</span></span>

<span data-ttu-id="a2d0c-104">Потребителите не могат да отварят отчети.</span><span class="sxs-lookup"><span data-stu-id="a2d0c-104">Users are unable to open reports.</span></span> <span data-ttu-id="a2d0c-105">"Нещо се е объркало.</span><span class="sxs-lookup"><span data-stu-id="a2d0c-105">"Something has gone wrong.</span></span> <span data-ttu-id="a2d0c-106">Проверете техническите подробности за повече подробности."</span><span class="sxs-lookup"><span data-stu-id="a2d0c-106">Check technical details for more details."</span></span>

<span data-ttu-id="a2d0c-107">**Причина**</span><span class="sxs-lookup"><span data-stu-id="a2d0c-107">**Cause**</span></span>

<span data-ttu-id="a2d0c-108">Отчетите не се зареждат в UCI с грешка "Дескриптор на формуляр е null или не е дефиниран."</span><span class="sxs-lookup"><span data-stu-id="a2d0c-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="a2d0c-109">Отчетите в UCI все още изискват наследени диалози, така че системата на клиента трябва да е разрешена *allowlegacydialogsembedding.*</span><span class="sxs-lookup"><span data-stu-id="a2d0c-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="a2d0c-110">**Решение**</span><span class="sxs-lookup"><span data-stu-id="a2d0c-110">**Solution**</span></span>

1. <span data-ttu-id="a2d0c-111">Отидете в **раздела Настройки >администриране > Системни настройки > Общи .**</span><span class="sxs-lookup"><span data-stu-id="a2d0c-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="a2d0c-112">Задайте "Разрешаване на вграждането на някои наследени диалогови прозорци в Унифициран интерфейс на браузъра клиент" на **Да**.</span><span class="sxs-lookup"><span data-stu-id="a2d0c-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
