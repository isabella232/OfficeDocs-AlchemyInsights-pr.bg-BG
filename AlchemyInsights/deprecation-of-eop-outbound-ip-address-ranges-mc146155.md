---
title: 1065 осъждане на EOP изходящи IP адрес rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404810"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="cc85b-102">Осъждане на EOP изходящи IP адреси</span><span class="sxs-lookup"><span data-stu-id="cc85b-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="cc85b-103">Ние сме открили потенциален проблем с вашата организация, които (ако не се коригира от 26 Октомври 2018) може да прекъсне потока от поща към локалната или външни дестинации.</span><span class="sxs-lookup"><span data-stu-id="cc85b-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="cc85b-104">Като преди това съобщава да опрости IP адреса диапазон управление, ние сте консолидирали Exchange онлайн защита (EOP) IP адрес обхвати, които се използват за изпращане и получаване на имейл от Office 365.</span><span class="sxs-lookup"><span data-stu-id="cc85b-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="cc85b-105">Нашият анализ показва, че един или повече от външни email източници или дестинации, които сте конфигурирали в поща поток съединители не приема връзки от IP адрес обхвати показано [тук](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="cc85b-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="cc85b-106">Действа преди 26 октомври да се гарантира тези източници и местоназначения ще приеме връзки към и от всички [публикувани EOP IP адреси](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="cc85b-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="cc85b-107">За повече информация за тази промяна моля вижте съобщение център мнения [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="cc85b-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="cc85b-108">**Забележка**: Ако сте използвали преди това IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайна точка, вие също трябва да мигрират към новата уеб услугите за автоматизиране на тези видове актуализации.</span><span class="sxs-lookup"><span data-stu-id="cc85b-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="cc85b-109">За повече информация вижте [Office 365 endpoint категории и Office 365 IP адрес и URL адрес на уеб услуга](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="cc85b-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
