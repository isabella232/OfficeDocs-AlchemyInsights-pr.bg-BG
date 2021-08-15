---
title: Изтриване на клиент
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993882"
---
# <a name="delete-tenant"></a>Изтриване на клиент

За да изтриете Azure AD, уверете се, че:
- Вие сте глобален администратор в указателя.
- НЕ сте влезли с акаунт, който има указателя по подразбиране, contoso.onmicrosoft.com в акаунта за влезли, като например admin@contoso.onmicrosoft.com.
- Премахнете всички активни приложения в указателя преди изтриването. За да премахнете активните приложения, отидете до Регистрации на приложения и премахнете съществуващите приложения.
- Няма активни абонаменти за никакви онлайн услуги на Microsoft, като например Microsoft Azure, Office 365 Azure AD Premium свързани в указателя. Можете да прехвърлите абонаментите си или да ускорите отмяната на активни абонаменти чрез поддръжката и фактурирането на Azure. Научете повече за това как да отмените Office 365 абонаменти и абонаменти за Azure. За указания относно асоциирането или добавянето на съществуващ абонамент към клиент вижте Свързване или добавяне на абонамент за [Azure към вашия клиент на Azure AD.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Няма активен лиценз. За да премахнете лицензи, вижте [Как да премахнете абонамента за премахване на лиценз](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Няма други активни потребители в указателя освен вас като глобален администратор, когато се опитвате да изтриете Azure AD. Премахнете всички други активни потребители и всички зависимости от име на домейн по избор в клиента също ще трябва да бъдат премахнати, като например потребители, създадени с admin@contoso.com.

За по-подробни стъпки как да:
- Изтрийте "Azure Active Directory" или "абонамент", вижте [Изтриване Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Премахване на приложения в указателя вижте [Премахване на приложения](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
