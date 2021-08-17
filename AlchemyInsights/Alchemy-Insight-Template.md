---
title: същото като име на файл е най-добре
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312814"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Задължително Alchemy Header H1, H2 не работи".
Най-добри практики и насоки за автори на Алхимия:

1. **Не влагайте Alchemy Прозрения папки – това** ще прекъсне структурата на URL адреса. Търсим да поправим това.
1. Файловете в **папката AlchemyInsights** трябва да имат малки имена на файлове с тирета за интервали ex. **_how-to-enable-litigation-hold_**.
    1. Включете ИД на правило или ИД на група от [портала за партньори на Alchemy](https://alchemyportal.azurewebsites.net) в полето ms.custom. ex. ***ms.custom: 100021***
1. Използвайте останалата част от метаданните в горната част на този файл като шаблон.
1. В [портала за партньори на Alchemy](https://alchemyportal.azurewebsites.net)отидете надолу до секцията Заглавие на **Customer Insight:** и го използвайте като отправна точка за заглавието на H1 за прозренията. 

**Забележка:** Alchemy Прозрения MUST има само един H1 в горната част или ще се прекъсне в производството. H2s не рендират така, че използвайте **получер** или други конвенции, за да пишете отделни секции.
1. След това попълнете текста на тялото с помощта на черновата в Customer Insights на страницата Правило за алхимия
    1. Списъците с водещи символи са наред
    1. Номерирани списъци също
    1. **Получер** *и италиатичен* са a-ok
    1. Връзките винаги трябва да са **или "връзки към уеб"/външни** ИЛИ дълбоки връзки към елементи на **потребителския интерфейс,** а не вътрешни връзки.
    1. Картините не се поддържат официално в момента, но са в пътната карта.

И това вече е твърде дълго. Най-добрата практика е около 400 знака ---------------------------------

След като съдържанието ви е готово, издърпайте го в живия клон. След това отидете в портала [на партньора на Alchemy](https://alchemyportal.azurewebsites.net) и въведете името на файла в полето url адрес. 