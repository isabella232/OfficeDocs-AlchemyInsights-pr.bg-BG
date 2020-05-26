---
title: 'AIP скенер: инсталация и конфигурация'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357353"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP скенер: инсталация и конфигурация

**За да инсталирате AIP скенера, следвайте препоръчителните указания:**

1. Ако надстройвате и не извършвате инсталация на чисто, уверете се, че сте следвали указанията за [надстройване на скенера](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) за защита на информацията на Azure и за обединен клиент за етикетиране, вижте [надстройване на скенера за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Проверете дали отговаряте на [всички изисквания за настройките на защитната стена и мрежовата инфраструктура](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Уверете се, че [правилата ви са зададени](https://docs.microsoft.com/azure/information-protection/configure-policy) на автоматично етикетиране или имат етикет по подразбиране в правилата.
4. Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [типове файлове, поддържани от клиента azure защита информация](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: [Промяна на нивото на защита на файлове](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)по подразбиране .
5. Проверете дали потребителският акаунт е конфигуриран да изпълнява услугата на скенера, има разрешения за достъп до всички конфигурирани хранилища.
6. Ако все още имате проблеми, моля, експортирайте регистрационните файлове на скенера и ги добавете към вашия билет за поддръжка.

**Експортиране на регистрационни файлове на скенера за защита на информация на Azure**

1. Навигирайте до %localappdata%\Microsoft\MSIP в контекста на потребителя, изпълняващ услугата на скенера.
2. Zip цялото съдържание в папката MSIP.
3. Запазете регистрационните файлове на вашия избор на местоположение и ги прикачете към заявката за услуги.
4. Можете също да използвате [експортиране-AIPLogs -OnuseOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**За допълнителна информация вижте**:
- [Разполагане на скенера за защита на информация на Azure за автоматично класифициране и защита на файлове](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Задайте и използвайте параметъра маркер за задаване aIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Стартиране на цикъл на откриване и преглед на отчети за скенера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Преглед на документацията за защита на информация за Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Изисквания за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Изтегляне на клиент абсбдис на информация за Azure](https://www.microsoft.com/download/details.aspx?id=53018)
