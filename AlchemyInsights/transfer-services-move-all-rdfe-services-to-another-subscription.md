---
title: Услуги за прехвърляне – преместване на всички услуги на RDFE към друг абонамент
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691929"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Услуги за прехвърляне – преместване на всички услуги на RDFE към друг абонамент

**"Премахни ресурсите"**

Ресурсите на Azure могат да бъдат преместени към друг абонамент за Azure или група ресурси под един и същ абонамент чрез Azure Portal, Azure PowerShell, Azure CLI или останалата част от API за преместване на ресурси.

За да можете да прехвърлите ресурси, вижте:

- [Контролен списък, преди да преместите ресурсите](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Услуги, които могат да бъдат преместени](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Как се проверява движението](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Ръководство за движение за услуги](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

За да премествате съществуващи ресурси към друга група ресурси или абонамент, можете да използвате:

- [Портал на Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Урок: [премествате ресурси на Azure към друга група ресурси или абонамент](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Отстраняване на грешки при диспечера за ресурси на Azure**

Вижте статиите по-долу, за да научите за някои често срещани грешки при разполагане на Azure и да получите информация за отстраняването им. Ако не можете да намерите кода на грешката за грешката си за разполагане, вижте [намиране на код на грешка](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Отстраняване на грешки при разполагане](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Отстраняване на неизправности при преместване на ресурси на Azure към нова група ресурси или абонамент](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Имайте предвид, че ако искате да надстроите своя абонамент за Azure, като например да преминете от свободен към платено, ще трябва да конвертирате абонамента си.

- За да надстроите безплатно изпробване, вижте [надстройване на вашия безплатен пробен период или абонамент за Microsoft за Azure, за да можете да плащате по-нататък](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- За да промените акаунт за плащане като за отиване, вижте [Промяна на вашия абонамент за вашия Azure Pay-do-Go за друго предложение](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).

**За да добавите или свържете абонамент за Azure към вашия клиент на Azure Active Directory:**

1. Впишете се и изберете абонамента, който искате да използвате, от страницата ' ' рецепти ' ' [в портала на Azure](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).
2. Изберете **Промяна на справочен указател**.
3. Прегледайте всички предупреждения, които се появяват, след което изберете **Промяна**.
4. Справочникът се променя за абонамента и ще получите съобщение за успех.
5. Използвайте превключвателя *Directory* , за да отидете в новия си указател. Възможно е да са необходими до 10 минути, за да се покаже всичко правилно.

**Препоръчвани документи**

- [Прехвърляне на собствеността върху абонамент за Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Преминаване на ресурси към нова група ресурси или абонамент](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Управление на ресурси чрез портала на Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
