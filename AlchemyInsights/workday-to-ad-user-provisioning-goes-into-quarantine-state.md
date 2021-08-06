---
title: Работен ден за ad User Provisioning отива в състояние на карантина
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
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036481"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Работен ден за ad User Provisioning отива в състояние на карантина

**Работен ден за ad User Provisioning отива в състояние на карантина и не се създават потребители в AD**

Задачата За осигуряване на потребители от работен ден в AD е преминала в състояние на карантина и регистрационните файлове за проверка показват събития за неуспешно експортиране със съобщението за **грешка Грешка: OperationsError-SvcErr: Възникна грешка в операцията. Не е конфигурирана по-висша препратка за справочната услуга. Следователно справочната услуга не може да издава препратки към обекти извън тази гора.** Тази грешка обикновено се показва, ако контейнерът на Active Directory OU не е настроен правилно или ако има проблеми със съпоставянето на изрази, използвано за **родителDistinguishedName**.

Проверете параметъра OU по подразбиране **за нови** потребители за печатни грешки. Уверете се, че зададеният OU вече съществува във вашата AD. Ако използвате **parentDistinguishedName в съпоставянето** на атрибути, уверете се, че той винаги се оценява на известен контейнер в домейна AD. Проверете събитието Експортиране в регистрационните файлове за проверка, за да видите генерираната стойност.

За повече подробности относно конфигурирането на работния ден за автоматизирано осигуряване вижте [Урок: Конфигуриране на работен ден за автоматично осигуряване от потребителя](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

