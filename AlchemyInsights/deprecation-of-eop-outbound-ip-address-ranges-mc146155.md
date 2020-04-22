---
title: 1065 Осъждане на eOP изходящIP адрес диапазониMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704586"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="f045a-102">Осъждане на изходящи ip адреси на EOP</span><span class="sxs-lookup"><span data-stu-id="f045a-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="f045a-103">Установихме потенциален проблем с вашата организация, който (ако не бъде коригиран до 26 октомври 2018 г.) може да прекъсне потока на пощата до локалните или външни дестинации.</span><span class="sxs-lookup"><span data-stu-id="f045a-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="f045a-104">Както вече са съобщени, за да се опрости IP адрес обхват управление, ние консолидираме Exchange Online Защита (EOP) IP адреси, които се използват за изпращане и получаване на имейл извън Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f045a-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="f045a-105">Нашият анализ показва, че един или повече външни източници на имейли или дестинации, които сте конфигурирали в конекторите за пощенски поток не приемат връзки от ip адресите, показани [тук](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="f045a-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f045a-106">Действие преди 26 октомври, за да се гарантира, че тези източници и дестинации ще приемат връзки към и от всички [публикувани Ip адреси на EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="f045a-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f045a-107">За повече информация относно тази промяна вижте Центъра за съобщения [тамненияMC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="f045a-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="f045a-108">**Забележка:** Ако преди това сте използвали IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайни точки, трябва също да мигрирате към новите уеб услуги за автоматизиране на тези типове актуализации.</span><span class="sxs-lookup"><span data-stu-id="f045a-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="f045a-109">За повече информация вижте [Категории теории за крайни точки на Microsoft 365 и Microsoft 365 IP адрес и уеб услуга за URL адреси](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="f045a-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
