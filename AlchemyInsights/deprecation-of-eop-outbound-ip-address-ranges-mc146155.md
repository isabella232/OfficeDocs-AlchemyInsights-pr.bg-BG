---
title: 1065 за отхвърляне на EOP изходящ IP адрес rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806784"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7a6cd-102">Отхвърляне на диапазони от IP адреси за EOP</span><span class="sxs-lookup"><span data-stu-id="7a6cd-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7a6cd-103">Засякохме потенциален проблем с вашата организация, който (ако не е коригиран до 26 Октомври 2018), може да прекъсне движението на пощата към локалните или външните ви дестинации.</span><span class="sxs-lookup"><span data-stu-id="7a6cd-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7a6cd-104">Както е съобщено по-рано, за да опростите управлението на диапазони от IP адреси, обединяваме диапазоните от IP адреси за Exchange Online Protection (EOP), които се използват за изпращане и получаване на имейли извън Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7a6cd-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="7a6cd-105">Нашият анализ показва, че един или повече от външните имейл източници или дестинации, които сте конфигурирали в конекторите за пощенския поток, не приемат връзки от диапазоните от IP адреси, показани [тук](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7a6cd-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7a6cd-106">Действайте преди 26 октомври, за да сте сигурни, че тези източници и дестинации ще приемат връзки към и от всички [публикувани IP адреси на EoP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7a6cd-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7a6cd-107">За повече информация относно тази промяна вижте центъра за съобщения, публикациите на [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7a6cd-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="7a6cd-108">**Забележка**: Ако преди това сте използвали IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайна точка, можете също да мигрирате към новите уеб услуги за автоматизиране на тези типове актуализации.</span><span class="sxs-lookup"><span data-stu-id="7a6cd-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7a6cd-109">За повече информация вижте [категории за крайна точка на microsoft 365 и microsoft 365 IP Address и URL уеб услуга](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7a6cd-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
