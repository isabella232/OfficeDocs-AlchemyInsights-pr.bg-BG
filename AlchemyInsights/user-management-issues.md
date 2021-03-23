---
title: Проблеми при управление на потребители
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034941"
---
# <a name="user-management-issues"></a>Проблеми при управление на потребители

**Какво се случва с текущите присвоени потребители към приложението, ако забраня свойството "задължително потребителско задание" (Задайте това свойство на "не")?**

Забраняването на **изискваното потребителско задание** не оказва влияние върху присвоените в момента потребители. Забраняването на това свойство ще позволява на всички потребители достъп до приложението. Всички изброени потребители и тези потребители, присвоени на групи в приложението, все още ще бъдат валидни.

- За да ограничите приложението до определен набор от потребители, вижте [ограничаване на приложението AZURE ad към набор от потребители – платформа за самоличност на Microsoft | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- За да присвоите потребители и групи, към корпоративни приложения в Azure Active Directory (Azure AD), в портала на Azure или с помощта на PowerShell вижте [управление на задачата на потребителите за приложение в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).
- За да делегирате разрешения за създаване и управление на приложения, вижте [делегиране на разрешения на администратор за управление на приложения – AZURE ad | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Скрийте определени корпоративни приложения от потребители** – Използвайте следните стъпки, за да скриете всички приложения на Microsoft 365 от панела " **моите приложения** ". Приложенията все още ще бъдат видими в портала на Office 365.

 1. Влезте в портала на Azure като глобален администратор за вашия указател. 
 2. Изберете **Azure Active Directory**. 
 3. Изберете **потребители**. 
 4. Изберете **потребителски настройки**. 
 5. Под **корпоративни приложения** щракнете върху **управление как се стартират крайните потребители и преглеждате техните приложения**. 
 6. За **потребителите могат да виждат само приложенията на office 365 в портала на office 365**, щракнете върху **да**. 
 7. Щракнете върху **Запиши**. 
 8. За повече информация вижте [скриване на корпоративната заявка от потребителския опит в AZURE ad | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Ако предлагате софтуер като приложение Service (SaaS) за много организации, можете да конфигурирате приложението си да приема влизане от всеки клиент на Azure Active Directory (Azure AD). Тази конфигурация се нарича "правене на вашето приложение Multi-клиент". Потребителите във всеки клиент на Azure AD ще могат да влизат в приложението, след като са съгласни да използват своя акаунт в приложението. За повече информация вижте [Създаване на приложения, които влизат в AZURE ad потребители – платформа за самоличност на Microsoft | Документи на Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Как може един краен потребител да получи достъп до приложението, след като му е присвоено това приложение?**

Всяко приложение в Блейд на Enterprise Application има връзка за крайни потребители за достъп. Потребителите могат също да имат достъп до приложението чрез портала на **моите приложения** по лесния начин.

- **Искате да знаете кои приложения и тип приложения се използват от потребителите?**

Можете да изтеглите отчетите за влизане за последните 30 дни от **portal.azure.com > Azure Active directory> Signins> изтегляне на отчети**.

- Научете как да [предоставите съгласие на клиента широк администратор за приложение и да](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) [конфигурирате как крайните потребители да се съгласяват с приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- Разберете [Как действа съгласие](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) и [управление на съгласието за приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


