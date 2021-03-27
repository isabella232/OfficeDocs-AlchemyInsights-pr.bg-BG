---
title: Концепции за разширено удостоверяване, приложими за Microsoft Edge
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398540"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="db03a-102">Концепции за разширено удостоверяване, приложими за Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="db03a-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="db03a-103">Следват концепциите за разширено удостоверяване, които са приложими за Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="db03a-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="db03a-104">**Проактивно удостоверяване**</span><span class="sxs-lookup"><span data-stu-id="db03a-104">**Proactive Authentication**</span></span>

<span data-ttu-id="db03a-105">Когато разрешите правилата [proactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge ще се опита проактивно да удостовери влезлите потребители чрез услугите на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="db03a-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="db03a-106">На равни интервали той ще използва онлайн услуга, за да провери за актуализиран манифест, който съдържа конфигурацията, регулираща проактивното удостоверяване.</span><span class="sxs-lookup"><span data-stu-id="db03a-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="db03a-107">Предимства: Проактивното удостоверяване позволява удостоверяване към ключови услуги, като например страницата с нов раздел на Office.</span><span class="sxs-lookup"><span data-stu-id="db03a-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="db03a-108">Освен това, ако Bing се използва като търсачка, проактивното удостоверяване подобрява производителността на адресната лента и помага за генерирането на резултати от търсенето, персонализирани за нуждите на вашата фирма.</span><span class="sxs-lookup"><span data-stu-id="db03a-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="db03a-109">**Windows Hello CredUI за NTLM удостоверяване**</span><span class="sxs-lookup"><span data-stu-id="db03a-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="db03a-110">Ако еднократна идентификация (SSO) не е налична, когато уеб сайт се опита да подпише потребителя чрез NTLM или Negotiate механизъм, тази функция ще позволи на потребителя да сподели идентификационните данни на операционната система с уеб сайта и да отговори на предизвикателството за удостоверяване с помощта на потребителския интерфейс на Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="db03a-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="db03a-111">Този поток за влизане ще се показва само в Windows 10 и само за потребители, които не получават SSO по време на NTLM или предизвикателство за Negotiate.</span><span class="sxs-lookup"><span data-stu-id="db03a-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="db03a-112">**Използване на записани пароли за автоматично влизане**</span><span class="sxs-lookup"><span data-stu-id="db03a-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="db03a-113">Потребителите, които записват пароли в Microsoft Edge, могат да активират автоматично влизане в уеб сайтове, където са записали идентификационни данни.</span><span class="sxs-lookup"><span data-stu-id="db03a-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="db03a-114">Потребителите могат да включват или изключват тази функция в edge://settings/passwords и можете да я конфигурирате в правилата за [управление на](https://go.microsoft.com/fwlink/?linkid=2134622) пароли.</span><span class="sxs-lookup"><span data-stu-id="db03a-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
