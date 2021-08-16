---
title: 1065 Обезценка на диапазони за изходящ IP адрес на EOPMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031251"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Отстраняване на диапазони от изходящ IP адрес на EOP

Открихме потенциален проблем с вашата организация, който (ако не е коригиран до 26 октомври 2018 г.) може да прекъсне пощенския поток до вашите локални или външни местоназначения. Както беше съобщено по-рано, за да опростите управлението на диапазона на IP адресите, консолидираме диапазоните от IP адреси на Exchange Online Protection (EOP), които се използват за изпращане и получаване на имейл извън Microsoft 365. Нашият анализ показва, че един или повече от външните имейл източници или местоназначения, които сте конфигурирали в конекторите за пощенския поток, не приемат връзки от диапазоните на IP адресите, показани [тук.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Действайте преди 26 октомври, за да гарантирате, че тези източници и местоназначения ще приемат връзки към и от [всички публикувани IP адреси на EOP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

За повече информация относно тази промяна вижте Публикации в центъра за съобщения [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620) [или MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Забележка:** Ако преди това сте използвали IP или URL публикуване чрез HTML, XML и RSS за актуализации на крайни точки, трябва също да мигрирате към новите уеб услуги за автоматизиране на тези типове актуализации. За повече информация [вж. Microsoft 365 крайни точки и Microsoft 365 IP адрес и уеб услуга за URL адреси.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)
