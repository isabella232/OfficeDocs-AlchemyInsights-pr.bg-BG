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
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Осъждане на изходящи ip адреси на EOP

Установихме потенциален проблем с вашата организация, който (ако не бъде коригиран до 26 октомври 2018 г.) може да прекъсне потока на пощата до локалните или външни дестинации. Както вече са съобщени, за да се опрости IP адрес обхват управление, ние консолидираме Exchange Online Защита (EOP) IP адреси, които се използват за изпращане и получаване на имейл извън Microsoft 365. Нашият анализ показва, че един или повече външни източници на имейли или дестинации, които сте конфигурирали в конекторите за пощенски поток не приемат връзки от ip адресите, показани [тук](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Действие преди 26 октомври, за да се гарантира, че тези източници и дестинации ще приемат връзки към и от всички [публикувани Ip адреси на EOP](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

За повече информация относно тази промяна вижте Центъра за съобщения [тамненияMC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)или [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Забележка:** Ако преди това сте използвали IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайни точки, трябва също да мигрирате към новите уеб услуги за автоматизиране на тези типове актуализации. За повече информация вижте [Категории теории за крайни точки на Microsoft 365 и Microsoft 365 IP адрес и уеб услуга за URL адреси](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
