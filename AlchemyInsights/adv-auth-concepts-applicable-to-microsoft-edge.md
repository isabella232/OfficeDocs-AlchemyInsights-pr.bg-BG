---
title: Разширени понятия за удостоверяване, приложими за Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573281"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="caaf8-102">Разширени понятия за удостоверяване, приложими за Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="caaf8-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="caaf8-103">По-долу са разширените понятия за удостоверяване, които са приложими за Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="caaf8-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="caaf8-104">**Proactive удостоверяване**</span><span class="sxs-lookup"><span data-stu-id="caaf8-104">**Proactive Authentication**</span></span>

<span data-ttu-id="caaf8-105">Когато активирате правилата за [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge ще се опита да удостовери по-активно влезлите потребители чрез Microsoft Services.</span><span class="sxs-lookup"><span data-stu-id="caaf8-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="caaf8-106">През определени интервали от време той ще използва онлайн услуга, за да провери за актуализиран манифест, който съдържа конфигурацията, управляваща proactive удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="caaf8-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="caaf8-107">Ползи: проактивното удостоверяване позволява удостоверяване на ключовите услуги, като например страницата на Office New TAB.</span><span class="sxs-lookup"><span data-stu-id="caaf8-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="caaf8-108">Освен това, ако Bing се използва като търсачка, проактивното удостоверяване подобрява производителността на адресната лента и помага за генериране на резултати от търсене, които са персонализирани за нуждите на вашата фирма.</span><span class="sxs-lookup"><span data-stu-id="caaf8-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="caaf8-109">**Windows Hello CredUI за NTLM удостоверяване**</span><span class="sxs-lookup"><span data-stu-id="caaf8-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="caaf8-110">Ако еднократната идентификация (SSO) не е налична, когато уеб сайтът се опитва да влезе на потребителя чрез NTLM или договорния механизъм, тази функция ще позволява на потребителя да споделя идентификационните данни за операционната система с уеб сайта и да удовлетвори предизвикателството за удостоверяване с помощта на потребителския интерфейс на Windows Hello CRED.</span><span class="sxs-lookup"><span data-stu-id="caaf8-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="caaf8-111">Този поток за влизане ще се показва само в Windows 10 и само за потребители, които не получават SSO по време на NTLM или договорени предизвикателства.</span><span class="sxs-lookup"><span data-stu-id="caaf8-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="caaf8-112">**Използване на запазени пароли за автоматично влизане**</span><span class="sxs-lookup"><span data-stu-id="caaf8-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="caaf8-113">Потребителите, които записват пароли в Microsoft Edge, могат да разрешат автоматичното влизане на уеб сайтове, където имат записани идентификационни данни.</span><span class="sxs-lookup"><span data-stu-id="caaf8-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="caaf8-114">Потребителите могат да включват или изключват тази функция в edge://settings/passwords и можете да го конфигурирате в правилата за [управление на пароли](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="caaf8-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
