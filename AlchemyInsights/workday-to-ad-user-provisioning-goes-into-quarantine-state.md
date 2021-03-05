---
title: Осигуряването на работното ви работно _ работно
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480966"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="cd838-102">Осигуряването на работното ви работно _ работно</span><span class="sxs-lookup"><span data-stu-id="cd838-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="cd838-103">**Осигуряването на работното ви работното си работното на потребителите преминава в карантинни състояния и няма създадени потребители в AD**</span><span class="sxs-lookup"><span data-stu-id="cd838-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="cd838-104">Работата за осигуряване на работния ден на AD потребители е изминала в карантинно състояние и регистрационните файлове за проверка показват неуспешни събития при експортиране със съобщение за грешка **: OperationsError-SvcErr: Възникна грешка в операция. За справочната услуга не е конфигурирана превъзходна препратка. Следователно справочната услуга не е в състояние да издава препратки към обекти извън тази гора**.</span><span class="sxs-lookup"><span data-stu-id="cd838-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="cd838-105">Тази грешка обикновено се показва, ако контейнерът на Active Directory не е зададено правилно или има проблеми с използваното съпоставяне на изрази за **parentDistinguishedName**.</span><span class="sxs-lookup"><span data-stu-id="cd838-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="cd838-106">Проверете настройките по подразбиране за **нови потребители** за правописни грешки.</span><span class="sxs-lookup"><span data-stu-id="cd838-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="cd838-107">Уверете се, че указаната ОЕ вече съществува във вашата реклама.</span><span class="sxs-lookup"><span data-stu-id="cd838-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="cd838-108">Ако използвате **parentDistinguishedName** в съпоставяне на атрибути, уверете се, че той винаги оценява известен контейнер в рамките на рекламния домейн.</span><span class="sxs-lookup"><span data-stu-id="cd838-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="cd838-109">Проверете събитието за експортиране в регистрационните файлове за проверка, за да видите генерираната стойност.</span><span class="sxs-lookup"><span data-stu-id="cd838-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="cd838-110">За повече информация за конфигурирането на работен ден за автоматизирано осигуряване вижте [урок: Конфигуриране на работен ден за автоматично осигуряване на потребителя](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span><span class="sxs-lookup"><span data-stu-id="cd838-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

