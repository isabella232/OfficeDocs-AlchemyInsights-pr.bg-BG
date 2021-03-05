---
title: Конфигуриране на услугата за синхронизиране на мим
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480900"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="ce1c2-102">Конфигуриране на услугата за синхронизиране на мим</span><span class="sxs-lookup"><span data-stu-id="ce1c2-102">Configure MIM Sync service</span></span>

<span data-ttu-id="ce1c2-103">Услугата за синхронизация на Microsoft Identity Manager (мим) е компонент на мим.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="ce1c2-104">Това е централизирана локална услуга, която съхранява и интегрира информация за организации, които имат множество локални указатели и бази данни.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="ce1c2-105">Възможно е да успеете да отстраните проблема си с мим Sync, ако проблемът е адресиран в скорошна актуализация за мим или е един от другите проблеми, упоменати в раздела по-долу.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="ce1c2-106">**Препоръчителни стъпки**</span><span class="sxs-lookup"><span data-stu-id="ce1c2-106">**Recommended steps**</span></span>

1. <span data-ttu-id="ce1c2-107">Уверете се, че използвате скорошна актуализация на мим Sync и проверете [бележките за изданието на мим за синхронизиране](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) , за да определите дали проблемът е разрешен в актуализация.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="ce1c2-108">Ако проблемът е с генеричните LDAP, Generic SQL, Lotus Domino или Web Services Connector, уверете се, че използвате скорошна актуализация на [генеричните конектори](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="ce1c2-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="ce1c2-109">Ако даден мим за синхронизиране спре с грешка, прегледайте таблицата с кодове на [грешки при изпълнение](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) , за да определите потенциалните причини.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="ce1c2-110">Ако изпълнението спира с **разширение-DLL-изключение**, след това щракнете върху тези думи, за да отворите прозореца **за свойства на обекта на конектора** , след което щракнете върху **проследяване на стека...** , за да видите повече информация за основната причина, както е описано в [разширение-DLL-изключение](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce1c2-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="ce1c2-111">Ако функцията за известяване при промяна на парола (PCNS) съобщава за **грешка 6025** в регистъра на събитията по време на синхронизирането на пароли, прегледайте справочника за отстраняване на неизправности при [Съобщаване за грешки в PCNS на 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce1c2-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="ce1c2-112">Ако пълната синхронизация с агента за управление на FIM услугата е бавна, Проверете настройката за **автоматично нарастване** за TempDB, както е описано в [отстраняване на неизправности или висящо пълно синхронизиране](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce1c2-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="ce1c2-113">Ако се сблъскате с грешка от спряно сървъра с Неуспешно създаване на уеб-услуги с помощта на агента за управление на FIM услуга, вижте [поддръжка-info: Неуспешно създаване-уеб-услуги](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) за общ преглед на причините.</span><span class="sxs-lookup"><span data-stu-id="ce1c2-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

