---
title: Хеширане на синхронизирането на пароли за услугата Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177366"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Хеширане на синхронизирането на пароли за услугата Domain

**Ако вашият екземпляр на Azure AD DS ви подкани да разрешите синхронизирането на хеширане с парола**

Ще срещнете сценарий, в който изпълнявате хибридна среда, в която потребителите ще се синхронизират от локалната среда за домейни на Azure Active Directory (AD DS). Този сценарий се среща, въпреки че имате парола за хеширане от локалния AD DS към вашия клиент на Azure AD.

**Причиняват**

Това се случва, защото Azure AD Connect по подразбиране не синхронизира наследени нови технологии за LAN Manager (NTLM) и Kerberos парола хеширане, които са необходими за Azure AD DS.

**Заобиколно решение** 

Ще трябва да конфигурирате Azure AD Connect, за да синхронизирате тези хеширане на пароли, необходими за NTLM и Kerberos удостоверяване.

След като Azure AD Connect е конфигурирана, за създаване на локален акаунт или за промяна на паролата, след което се синхронизират наследени хеширани пароли в Azure AD. Вижте [тук](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) за повече информация относно това и за насоки как да разрешите синхронизирането на пароли в AZURE AD DS хибридни среди.