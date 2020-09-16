---
title: 'Скенер на ПДИ: инсталиране и конфигуриране'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686631"
---
# <a name="aip-scanner-installation-and-configuration"></a>Скенер на ПДИ: инсталиране и конфигуриране

**За да инсталирате скенера на ПДИ, следвайте препоръчваните указания**:

1. Ако надстройвате и не извършвате инсталация на чисто, моля, уверете се, че сте следвали насоките за [надстройване на програмата за защита на данните на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) и за унифициран клиент за етикетиране вижте [надстройване на инструмента за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Проверете дали спазвате всички изисквания за [настройките на защитната стена и мрежова инфраструктура](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Уверете се, че [правилата ви са настроени](https://docs.microsoft.com/azure/information-protection/configure-policy) за автоматично етикетиране или имат етикет по подразбиране в правилата.
4. Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [типовете файлове, поддържани от клиента за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: [Промяна на нивото на защита по подразбиране на файлове](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Уверете се, че потребителският акаунт, конфигуриран за изпълнение на услугата Scanner, има разрешения за достъп до всички конфигурирани хранилища.
6. Ако все още имате проблеми, можете да експортирате регистрите на скенера и да ги добавите към своя билет за поддръжка.

**Експортиране на регистрационни файлове на скенера за защита на информацията на Azure**

1. Придвижете се до%localappdata%\Microsoft\MSIP под потребителския контекст, в който се изпълнява услугата Scanner.
2. Архивирайте цялото съдържание под папката MSIP.
3. Запишете регистрационните файлове по ваш избор и ги прикачете към вашата заявка за обслужване.
4. Можете също да използвате [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**За допълнителна информация вж**.:
- [Разполагане на скенера за защита на информацията на Azure за автоматично класифициране и защита на файлове](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Указване и използване на параметъра на маркера за Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Изпълнение на цикъл на откриване и преглед на отчети за скенера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Преглед на документацията за защита на информацията на Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Изисквания за информация за Azure Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Изтегляне на Azure за защита на информацията за клиента](https://www.microsoft.com/download/details.aspx?id=53018)
