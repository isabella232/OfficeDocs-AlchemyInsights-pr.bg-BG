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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564385"
---
# <a name="delete-tenant"></a>Изтриване на клиент

За да изтриете Azure AD, уверете се, че:
- Вие сте глобален администратор в указателя.
- НЕ сте влезли с акаунт, който има директорията по подразбиране, като например contoso.onmicrosoft.com, в акаунта за подписано-във, като например admin@contoso.onmicrosoft.com.
- Премахнете активните приложения в указателя, преди да ги изтриете. За да премахнете активните приложения, придвижете се до регистрации на приложения и премахнете съществуващите приложения.
- Няма активни абонаменти за каквито и да е онлайн услуги на Microsoft, като например Microsoft Azure, Office 365 или Azure AD Premium, свързани в указателя. Прехвърлете абонаментите си или Ускорете отмяната на активните абонаменти чрез поддръжка на Azure и фактуриране. Научете повече за това как да отмените абонамента за Office 365 и Azure. За насоки относно свързването или добавянето на съществуващ абонамент към клиент вижте [свързване или добавяне на абонамент за Azure към вашия клиент на AZURE ad](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Няма активни лицензи. За да премахнете лицензи, вижте [как да премахнете абонамент, за да премахнете лиценза](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Няма други активни потребители в директорията освен себе си като глобален администратор при опит за изтриване на Azure AD. Премахнете всички други активни потребители и всички зависимости в име на домейн по избор в клиента също ще трябва да бъдат премахнати, като например потребители, създадени с admin@contoso.com.

За повече подробности за стъпките относно:
- Изтрийте "Azure Active Directory" или "Абонамент", вижте [Изтриване на Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Премахване на приложения в указателя вижте [Премахване на приложения](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
