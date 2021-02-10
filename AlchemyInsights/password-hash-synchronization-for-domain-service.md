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
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="8927e-102">Хеширане на синхронизирането на пароли за услугата Domain</span><span class="sxs-lookup"><span data-stu-id="8927e-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="8927e-103">**Ако вашият екземпляр на Azure AD DS ви подкани да разрешите синхронизирането на хеширане с парола**</span><span class="sxs-lookup"><span data-stu-id="8927e-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="8927e-104">Ще срещнете сценарий, в който изпълнявате хибридна среда, в която потребителите ще се синхронизират от локалната среда за домейни на Azure Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="8927e-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="8927e-105">Този сценарий се среща, въпреки че имате парола за хеширане от локалния AD DS към вашия клиент на Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8927e-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="8927e-106">**Причиняват**</span><span class="sxs-lookup"><span data-stu-id="8927e-106">**Cause**</span></span>

<span data-ttu-id="8927e-107">Това се случва, защото Azure AD Connect по подразбиране не синхронизира наследени нови технологии за LAN Manager (NTLM) и Kerberos парола хеширане, които са необходими за Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="8927e-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="8927e-108">**Заобиколно решение**</span><span class="sxs-lookup"><span data-stu-id="8927e-108">**Workaround**</span></span> 

<span data-ttu-id="8927e-109">Ще трябва да конфигурирате Azure AD Connect, за да синхронизирате тези хеширане на пароли, необходими за NTLM и Kerberos удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="8927e-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="8927e-110">След като Azure AD Connect е конфигурирана, за създаване на локален акаунт или за промяна на паролата, след което се синхронизират наследени хеширани пароли в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8927e-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="8927e-111">Вижте [тук](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) за повече информация относно това и за насоки как да разрешите синхронизирането на пароли в AZURE AD DS хибридни среди.</span><span class="sxs-lookup"><span data-stu-id="8927e-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>