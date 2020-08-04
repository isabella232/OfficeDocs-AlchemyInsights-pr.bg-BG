---
title: Отстраняване на неизправности в разполагане на сертификат за удостоверяване на клиент
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554786"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="15fe5-102">Отстраняване на неизправности в разполагане на сертификат за удостоверяване на клиент</span><span class="sxs-lookup"><span data-stu-id="15fe5-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="15fe5-103">Профилите на intune NDES/SCEP и PKCS/PFX клиентските профили се използват често във връзка с други типове профили като WiFi, VPN и имейл, за да се даде възможност на потребителите да се идентифицират в корпоративните ресурси.</span><span class="sxs-lookup"><span data-stu-id="15fe5-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="15fe5-104">Когато тези типове профили са свързани с клиентски сертификат профил са зависи от успешното разполагане на този профил.</span><span class="sxs-lookup"><span data-stu-id="15fe5-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="15fe5-105">Първоначалната настройка на инфраструктурата и свързаната конфигурация на клиентски сертификат профил често изискват отстраняване на неизправности.</span><span class="sxs-lookup"><span data-stu-id="15fe5-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="15fe5-106">За поетапно ръководство за успешно настройване на NDES конектор и указания за отстраняване на неизправности за изолиране на проблеми с разполагане на сертификат вижте:</span><span class="sxs-lookup"><span data-stu-id="15fe5-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="15fe5-107">Конфигуриране на инфраструктура за поддръжка на SCEP с Intune</span><span class="sxs-lookup"><span data-stu-id="15fe5-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="15fe5-108">Общ преглед за отстраняване на SCEP сертификат профили с Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="15fe5-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="15fe5-109">Използвайте указаните скриптове PowerShell, за да проверите конфигурацията си.</span><span class="sxs-lookup"><span data-stu-id="15fe5-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="15fe5-110">За повече информация вижте Скриптове за проверка на [конектора на Intune сертификат](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="15fe5-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="15fe5-111">**Други често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="15fe5-111">**Other common issues**</span></span>

<span data-ttu-id="15fe5-112">**Когато се опитате да инсталирате конектора intune сертификат на NDES конектор сървър, получавам съобщение" "Паролата в искането за сертификат не може да бъде проверен. Може да е бил използван вече. Получете нова парола, за да изпратите тази заявка."**</span><span class="sxs-lookup"><span data-stu-id="15fe5-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="15fe5-113">Това съобщение означава, че трябва да изпълните инсталирането на сертификата като администратор на сертификата конектор.</span><span class="sxs-lookup"><span data-stu-id="15fe5-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="15fe5-114">В някои среди сървърите, където се изпълнява сертификат intune трябва да използвате прокси сървър за свързване с Intune и конектор за сертификат трябва да използвате прокси.</span><span class="sxs-lookup"><span data-stu-id="15fe5-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="15fe5-115">В някои случаи конектор NDES игнорира конфигурирани настройки на прокси и може да се наложи да конфигурирате настройките на прокси докато работи в контекста на защитата на LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="15fe5-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="15fe5-116">Решението е да стартирате Internet Explorer като система и конфигуриране на прокси в IE.</span><span class="sxs-lookup"><span data-stu-id="15fe5-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="15fe5-117">След рестартиране на услугата Intune конектор конекторът се свързва с Intune.</span><span class="sxs-lookup"><span data-stu-id="15fe5-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="15fe5-118">**Потребителските устройства вече не получават scep сертификати от NDES.**</span><span class="sxs-lookup"><span data-stu-id="15fe5-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="15fe5-119">Възможно е сертификатът за удостоверяване на клиента, издаден на сървъра NDES, и посочен по време на инсталирането на конектора NDES, е изтекъл или липсва.</span><span class="sxs-lookup"><span data-stu-id="15fe5-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="15fe5-120">За да разрешите:</span><span class="sxs-lookup"><span data-stu-id="15fe5-120">To resolve:</span></span> 
 
1. <span data-ttu-id="15fe5-121">Деинсталирайте конектора NDES.</span><span class="sxs-lookup"><span data-stu-id="15fe5-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="15fe5-122">Използвайте тези данни, за да поискате нов сертификат за удостоверяване на клиент или удостоверяване на сървъра:</span><span class="sxs-lookup"><span data-stu-id="15fe5-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="15fe5-123">Тема: CN = външен fqdn</span><span class="sxs-lookup"><span data-stu-id="15fe5-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="15fe5-124">Алтернативно име на обекта (и двете се изисква): DNS=външен fqdn, DNS =вътрешен fqdn</span><span class="sxs-lookup"><span data-stu-id="15fe5-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="15fe5-125">Преинсталирайте конектора NDES с новия сертификат.</span><span class="sxs-lookup"><span data-stu-id="15fe5-125">Reinstall the NDES connector with the new certificate.</span></span>