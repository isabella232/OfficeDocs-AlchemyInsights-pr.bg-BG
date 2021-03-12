---
title: Набор реплики
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713370"
---
# <a name="replica-set"></a><span data-ttu-id="d9b34-102">Набор реплики</span><span class="sxs-lookup"><span data-stu-id="d9b34-102">Replica set</span></span>

<span data-ttu-id="d9b34-103">AADDS се нарича също като управляван домейн.</span><span class="sxs-lookup"><span data-stu-id="d9b34-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="d9b34-104">Това е действително два домейнови контролера, които се изпълняват и поддържат от сървъра.</span><span class="sxs-lookup"><span data-stu-id="d9b34-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="d9b34-105">Двете домейнови контролери включват една основна DC и една репликация DC.</span><span class="sxs-lookup"><span data-stu-id="d9b34-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="d9b34-106">Архивите в AADDS (управляван домейн) са автоматизиран процес, управляван от платформата Azure.</span><span class="sxs-lookup"><span data-stu-id="d9b34-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="d9b34-107">В случай че има проблем с вашия управляван домейн, поддръжката на Azure може да ви помогне да възстановите от архивно копие.</span><span class="sxs-lookup"><span data-stu-id="d9b34-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="d9b34-108">Създавате всеки набор реплики във виртуална мрежа.</span><span class="sxs-lookup"><span data-stu-id="d9b34-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="d9b34-109">Всеки виртуален мрежа трябва да бъде взиран във всяка друга виртуална мрежа, която подслонява набора от реплики за управляван домейн.</span><span class="sxs-lookup"><span data-stu-id="d9b34-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="d9b34-110">Тази конфигурация създава топология на мрежестата мрежа, която поддържа репликация на справочен указател.</span><span class="sxs-lookup"><span data-stu-id="d9b34-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="d9b34-111">Една виртуална мрежа може да поддържа множество набори реплики, при условие че всеки набор реплики е в различна виртуална подмрежа.</span><span class="sxs-lookup"><span data-stu-id="d9b34-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="d9b34-112">За повече информация относно набор реплики вижте [понятията](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)набори от реплики.</span><span class="sxs-lookup"><span data-stu-id="d9b34-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
