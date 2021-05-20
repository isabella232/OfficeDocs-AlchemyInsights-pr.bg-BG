---
title: Създаване на потребител
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569700"
---
# <a name="create-user"></a>Създаване на потребител

**СЪОБЩЕНИЕ:**

- [Отстраняване на поддръжката за влизане в WebView от Google от 4 януари 2021 г.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Проверете дали приложенията ви може да бъдат засегнати, като [следвате указанията на Google](https://go.microsoft.com/fwlink/?linkid=2157323) за тестване на съвместимостта.
- Уверете се, че използвате системния уеб изглед или системния браузър, когато влизате в потребителите си с потребителски акаунти в Google. За повече информация вижте Проблеми [при влизане в приложения само с помощта на браузъра Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**Не мога да създам нов потребител в моя указател на Azure AD**

1. Уверете се, че сте упълномощени да създадете нов стандартен потребител. Само ролята на глобален администратор или администратор на потребител в Azure Active Directory (AD) може да създаде нов стандартен потребител. Ако не сте в някоя от тези роли, помолете администратор да ви добави към една от тези роли или да създаде новия потребителски акаунт за вас.
1. Уверете се, че потребителското име е в домейн, който е проверен във вашата Azure AD. Ако не разполагате с проверени имена на домейни по избор във вашата Azure AD, можете да използвате първоначалния си домейн на Azure AD, който завършва с *.onmicrosoft.com.
1. Уверете се, че потребителското име е в домейн, който не е федерирани към Azure AD от вашата локална AD. Потребителите не могат да се добавят в облака с имена на домейни, които са федерирани от локални.
1. Уверете се, че никой друг потребител или контакт вече няма потребителското име, което искате да присвоите на новия потребител. Потребителските имена трябва да са уникални в Azure AD.
1. Вижте [Роли и администратори на Azure AD за](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) azure AD.
1. Вижте имената [на домейните](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) за azure AD.
1. Прегледайте [регистрационните файлове за](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) проверка, за да видите по-подробна информация за наскоро създаден или изтрит потребител, като например кой е изпълнил действието и кога.
1. За повече информация относно добавянето на нови потребители вижте [Използване на портала на Azure за създаване на нов потребител във вашата Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Административни роли на Azure AD:](/azure/active-directory/active-directory-assign-admin-roles)Разрешения за роли на администратор в Azure Active Directory
1. Можете също да [използвате Azure AD PowerShell, за да създадете нов потребител.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
