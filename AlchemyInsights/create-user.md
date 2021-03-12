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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743180"
---
# <a name="create-user"></a>Създаване на потребител

**СЪОБЩЕНИЕ**

- Отхвърляне [на поддръжката на WebView за влизане от Google, започваща на 4 януари, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) . Проверете дали вашите приложения могат да бъдат засегнати, като следвате [указанията на Google](https://go.microsoft.com/fwlink/?linkid=2157323) относно проверката за съвместимост.
- Уверете се, че използвате System WebView или системен браузър, когато влизате в своите потребители с потребителски акаунти за Google. За повече информация вижте [проблеми при влизане в приложения, които използват само браузъра Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).

**Не мога да създам нов потребител в директорията си на Azure AD**

1. Уверете се, че сте упълномощени да създадете нов стандартен потребител. Само ролята на глобален администратор или администратор на потребителя в Azure Active Directory (AD) може да създаде нов стандартен потребител. Ако не сте в една от тези роли, помолете администратор да ви добави към една от тези роли или за да създадете новия потребителски акаунт за вас.
1. Уверете се, че потребителското име е в домейн, който е проверен във вашата Azure AD. Ако нямате проверени имена на домейни по избор във вашата Azure AD, можете да използвате първоначалния домейн на Azure AD, който завършва на *. onmicrosoft.com.
1. Уверете се, че потребителското име е в домейн, който не е външен за Azure AD от вашата локална реклама. Потребителите не могат да бъдат добавяни в облака с имена на домейни, които са външни за локален.
1. Уверете се, че никой друг потребител или контакт вече не разполага с потребителското име, което искате да дадете на новия потребител. Потребителските имена трябва да бъдат уникални в Azure AD.
1. Вижте [ролите и администраторите на AZURE ad](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) за вашата Azure ad.
1. Вижте [имената на домейни](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) за вашата Azure ad.
1. Проверете [регистрационните файлове за проверка](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) , за да видите по-подробна информация за наскоро създаден или изтрит потребител, като този, който е извършил действието, и кога.
1. За повече информация относно добавянето на нови потребители вижте [използване на портала на Azure, за да създадете нов потребител във вашата AZURE ad](/azure/active-directory/active-directory-users-create-azure-portal).
1. [Административни роли на AZURE ad](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): разрешения за роля на администратор в Azure Active Directory
1. Можете също да [използвате AZURE ad PowerShell, за да създадете нов потребител](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).
