---
title: Блокиран съм от условен достъп с устройство, което е присъединен към домейн
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/20/2021
ms.locfileid: "51035234"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Блокиран съм от условен достъп с устройство, което е присъединен към домейн

**Силно Препоръчителни инструменти**

[Инструмент за отстраняване на неизправности при регистриране на устройства](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – инструментът, който помага за отстраняване на най-често срещаните проблеми при регистриране на устройства.

[Скрипт за свързване на регистрационни устройства](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – скриптът, който помага да се гарантира, че устройството има достъп до крайните точки за регистрация на устройства под системния акаунт.

[Скрипт за изчистване на AZURE ad устройство](https://github.com/mzmaili/AzureADDeviceCleanup) – скриптът, който ви позволява да търсите и управлявате изхабени устройства във вашата среда.

Ето някои често срещани причини за условния достъп може да е неуспешно устройство, което е присъединен към домейн (хибридна Azure AD).

1. Няма **AZURE ad PRT на устройството** – трябва да се уверите, че устройството има маркер за основна обновяване на Azure ad (Prt). За повече информация за PRT вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

За да се уверите, че имате Azure AD PRT, можете да изпълните `dsregcmd/status` командата на устройството и да проверите дали "AzureAdPrt" е равно на "да".

Ако "AzureAdPrt" е "не", проверете следното:

- **Дали имате външна среда с AD FS и че е недостъпна за домашните мрежи на вашите потребители**: в този случай се уверете, че крайните точки на "usernamemixed" са достъпни от екстранет. Ако вашият AD FS е зад VPN мрежа, се уверете, че потребителите се свързват с VPN и повторно влизане в устройството. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Дали TPM на устройството е повреден и следователно не може да удостовери устройството**: Проверете "TPM. msc", за да видите дали състоянието на TPM е "Готово". Ако не е, изпълнете `dsregcmd/leave` и позволете на устройството да се присъедини повторно към AZURE ad. След това опитайте отново. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Използвате доставчик на самоличност, който не поддържа WS-Trust протокол**. Както е описано в нашите документи, хибридните Azure AD-Съединени устройства не могат да работят в този случай. Моля, Работете със своя доставчик на самоличност за поддръжка.

2. **Потребителите използват браузъра Chrome без акаунти за Windows 10** или разширение на Office, като браузърът **не използва автоматично ПВЕ в устройства, свързани с пад или хибриден пад**: това води до неуспех на всички базирани на устройства правила за достъп под условие, като се показва съобщение за грешка "нерегистрирано устройство". За да използвате правилно браузъра Chrome, трябва да инсталирате "акаунти за Windows 10" или "разширение на Office за браузъра на потребителите" чрез SCCM или в "Настройки". За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Ако не е възможно отдалечено да натискате разширението, уведомете потребителите, за да инсталирате ръчно едно от горните разширения, за да получите достъп до приложения зад условния достъп, базиран на устройства. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. **Устройството е правилно хибридно AZURE ad, но по невнимание е изтрито или забранено, поради което е необходимо да се синхронизират промените в AZURE ad Connect или от портала на Azure**: Ако това се случи, обектът на устройството вече не се разпознава като напълно присъединен план, въпреки че състоянието на "AzureAdJoined" и "PRT" се показва като валидно за устройството.

За да коригирате този проблем, изпълнете `dsregcmd/leave` на засегнатите устройства и им Позволете да се присъединят към AZURE ad. За повече информация вижте този [документ](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Ако вашите устройства са в Windows 10, актуализация на 1809, чрез прокси сървър за VPN/Cloud и вижте проблеми с "AzureAdPrt" или всяко приложение с проблем с SSO (Outlook не се свързва към пощенската кутия, въпреки че сте имали PRT), уверете се, че имате тази кръпка [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) или април сборна актуализация на [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) , за да предотвратите неуспехите на ПВЕ на тези машини.

















