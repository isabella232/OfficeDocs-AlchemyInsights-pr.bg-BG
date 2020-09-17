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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Отхвърляне на диапазони от IP адреси за EOP

Засякохме потенциален проблем с вашата организация, който (ако не е коригиран до 26 Октомври 2018), може да прекъсне движението на пощата към локалните или външните ви дестинации. Както е съобщено по-рано, за да опростите управлението на диапазони от IP адреси, обединяваме диапазоните от IP адреси за Exchange Online Protection (EOP), които се използват за изпращане и получаване на имейли извън Microsoft 365. Нашият анализ показва, че един или повече от външните имейл източници или дестинации, които сте конфигурирали в конекторите за пощенския поток, не приемат връзки от диапазоните от IP адреси, показани [тук](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Действайте преди 26 октомври, за да сте сигурни, че тези източници и дестинации ще приемат връзки към и от всички [публикувани IP адреси на EoP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

За повече информация относно тази промяна вижте центъра за съобщения, публикациите на [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Забележка**: Ако преди това сте използвали IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайна точка, можете също да мигрирате към новите уеб услуги за автоматизиране на тези типове актуализации. За повече информация вижте [категории за крайна точка на microsoft 365 и microsoft 365 IP Address и URL уеб услуга](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
