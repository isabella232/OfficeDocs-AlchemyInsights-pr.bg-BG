---
title: 'AIP скенер: инсталиране и конфигуриране'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934246"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP скенер: инсталиране и конфигуриране

**За да инсталирате AIP скенера, следвайте препоръчаните указания:**

1. Ако надстройвате и не извършвате чиста инсталация, уверете се, че сте следвали указанията за надстройване на [скенера за защита на информацията](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) на Azure и за унифициран клиент за етикети, вижте Надстройване на [скенера за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Уверете се, че спазвате всички изисквания [за настройки на защитната стена и мрежовата инфраструктура.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Уверете се, [че правилата ви са](https://docs.microsoft.com/azure/information-protection/configure-policy) зададени за автоматично етикети или имат етикет по подразбиране в правилата.
4. Уверете се, че съответният тип файл е конфигуриран за етикет/защита, както е описано в [Типове файлове, поддържани от клиента за защита на информацията в Azure.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Освен това, ако искате да промените поведението по подразбиране, следвайте тези указания: Промяна на [нивото на защита по подразбиране на файловете.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)
5. Уверете се, че потребителският акаунт, конфигуриран да изпълнява услугата за скенер, има разрешения за достъп до всички конфигурирани хранилища.
6. Ако все още имате проблеми, експортирайте регистрационните файлове на скенера и ги добавете към билета си за поддръжка.

**Експортиране на регистрационни файлове на скенера за защита на информацията в Azure**

1. Навигирайте до %localappdata%\Microsoft\MSIP под потребителския контекст, изпълняващ услугата за скенер.
2. Zip цялото съдържание под папката MSIP.
3. Запишете регистрационните файлове по ваш избор на местоположение и ги прикачете към вашата заявка за обслужване.
4. Можете също да използвате [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**За допълнителна информация вижте**:
- [Разполагане на скенера за защита на информацията в Azure за автоматично класифициране и защита на файлове](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Задаване и използване на параметъра "Маркер" за Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Изпълнение на цикъл на откриване и преглед на отчети за скенера](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Преглед на документацията за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Изисквания за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Изтегляне на клиента за защита на информацията в Azure](https://www.microsoft.com/download/details.aspx?id=53018)
