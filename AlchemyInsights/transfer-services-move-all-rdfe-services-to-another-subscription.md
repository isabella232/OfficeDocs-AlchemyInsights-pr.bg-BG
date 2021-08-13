---
title: Услуги за прехвърляне – Преместване на всички услуги на RDFE към друг абонамент
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
ms.openlocfilehash: 89217922b8b51f2548f9fff53bf80364c0e897b1d9b34bfb7016f0b0f197cf17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940022"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a>Услуги за прехвърляне – Преместване на всички услуги на RDFE към друг абонамент

**Преместване на ресурси**

Ресурсите на Azure могат да бъдат преместени в друг абонамент за Azure или група ресурси под един и същ абонамент с помощта на портала на Azure, Azure PowerShell, Azure CLI или REST API за преместване на ресурси.

Преди да можете да премествате ресурси, вижте:

- [Контролен списък преди преместване на ресурси](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [Услуги, които могат да бъдат преместени](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Как да проверите преместването](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [Указания за преместване за услуги](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

За да преместите съществуващи ресурси в друга група или абонамент за ресурси, можете да използвате:

- [Портал на Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [Azure PowerShell](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [Azure CLI](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [REST API](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

Урок: [Преместване на ресурси на Azure в друга група или абонамент за ресурси](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)

**Отстраняване на грешки с Azure Resource Manager**

Вижте статиите по-долу, за да научите за някои често срещани грешки при разполагане на Azure и да получите информация, за да ги отстраните. Ако не можете да намерите кода на грешката при разполагане, вижте Намиране [на код на грешка](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).

- [Отстраняване на грешки при разполагане](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [Отстраняване на неизправности при преместване на ресурси на Azure в нова група или абонамент за ресурси](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

Обърнете внимание, че ако искате да надстроите абонамента си за Azure, като например преминаване от безплатно към платено, ще трябва да конвертирате абонамента си.

- За да надстроите безплатна пробна версия, вижте Надстройване на вашия безплатен пробен период или абонамент за Microsoft Imagine Azure до [Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).
- За да промените акаунт за плащане в движение, вижте Промяна на абонамента ви за [Azure Pay-As-You-Go на друго предложение.](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)

**За да добавите или свържете абонамент за Azure към вашия Azure Active Directory клиент:**

1. Влезте и изберете абонамента, който искате да използвате от страницата [Абонаменти в портала на Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)
2. Изберете **Промяна на справочника**.
3. Прегледайте всички предупреждения, които се появяват, и след това **изберете Промяна**.
4. Указателят се променя за абонамента и ще получите съобщение за успех.
5. Използвайте *превключвателя на* справочника, за да отидете в новия указател. Може да отнеме до 10 минути, за да се покаже всичко правилно.

**Препоръчителни документи**

- [Прехвърляне на собствеността върху абонамент за Azure](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [Преместване на ресурси към нова група ресурси или абонамент](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [Управление на ресурси чрез портала на Azure](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
