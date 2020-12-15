---
title: Разрешаване на управлението на разходите
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/08/2020
ms.locfileid: "49676827"
---
# <a name="enable-cost-management"></a>Разрешаване на управлението на разходите

**Какво означават разходите за вашата организация?**

Организациите, използващи акаунти за корпоративно споразумение (EA) или споразумение за клиенти на Microsoft (МСА), могат да забранят достъпа до информацията за разходите и ценовата информация.

След като влезете в портала на Azure, той може да използва API за фактуриране, за да получи по програмен път фактури (след като сте се записали) и подробности за използването.

**Как да разрешите на допълнителни потребители да имат достъп до фактури**

1. Отидете на " **абонаменти" Блейд** в портала на Azure.
2. Изберете **фактури** и след това **достъп до фактури**.
3. Включване на Access, последвано от записване на промените, за да разрешите на потребителите в обхватните роли за абонаменти да изтеглят фактури.

> [!NOTE]
> Администраторът на акаунта може също да конфигурира да има фактури, изпратени по имейл. За да научите повече, вижте [получаване на фактурата ви по имейл](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Как се добавят потребители към ролята на четящия четец**

1. Отидете на " **абонаменти" Блейд** в портала на Azure.
2. Изберете **контрол на достъпа (IAM)** и след това щракнете върху **Добави**.
3. Изберете **Reader за фактуриране** в страницата **Изберете роля** .
4. Въведете имейла на потребителя, когото искате да поканите, и след това щракнете върху **OK** , за да изпратите поканата.
5. Следвайте инструкциите, предоставени в имейла за Поканване, за да влезете като четец за фактуриране. За повече информация вижте [предоставяне на достъп до фактуриране](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Препоръчвани документи**

- [Разрешаване на изгледи на DA и AO чрез портала на EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Разходи, включени в управлението на разходите](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Поддържани предложения на Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Преглед на разходите в анализа на разходите](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Предоставяне на достъп до информацията за фактуриране](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Проверяване на достъпа до клиентско споразумение на Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






