---
title: Отстраняване на неизправности при разполагане на сертификат за удостоверяване на клиент
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658975"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="730f2-102">Отстраняване на неизправности при разполагане на сертификат за удостоверяване на клиент</span><span class="sxs-lookup"><span data-stu-id="730f2-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="730f2-103">Потребителските профили за удостоверяване на NDES/SCEP и PKCS/PFX клиенти обикновено се използват съвместно с други типове профили, като например WiFi, VPN и имейл, за да позволят на потребителите да удостоверяват корпоративните ресурси.</span><span class="sxs-lookup"><span data-stu-id="730f2-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="730f2-104">Когато тези типове профили са свързани към профил на сертификат на клиент, той зависи от успешното разполагане на този профил.</span><span class="sxs-lookup"><span data-stu-id="730f2-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="730f2-105">Първоначалната настройка на инфраструктурата и асоциираната конфигурация на профила на сертификат на клиент често изисква отстраняване на неизправности.</span><span class="sxs-lookup"><span data-stu-id="730f2-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="730f2-106">За ръководство "стъпка по стъпка" за успешна настройка на NDES Connector и указания за отстраняване на неизправности за изолиране на проблеми при разполагане на сертификат вижте:</span><span class="sxs-lookup"><span data-stu-id="730f2-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="730f2-107">Конфигуриране на инфраструктурата за поддръжка на SCEP с настройка</span><span class="sxs-lookup"><span data-stu-id="730f2-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="730f2-108">Общ преглед за отстраняване на неизправности в профилите на SCEP с Microsoft</span><span class="sxs-lookup"><span data-stu-id="730f2-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="730f2-109">Използвайте адресираните скриптове на PowerShell, за да потвърдите конфигурацията.</span><span class="sxs-lookup"><span data-stu-id="730f2-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="730f2-110">За повече [информация вж.](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)</span><span class="sxs-lookup"><span data-stu-id="730f2-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="730f2-111">**Други често срещани проблеми**</span><span class="sxs-lookup"><span data-stu-id="730f2-111">**Other common issues**</span></span>

<span data-ttu-id="730f2-112">**Когато се опитам да инсталирам добавката за сертификат за извличане на NDES Connector Server, получавам съобщението "паролата в искането за сертификат не може да бъде проверена. Това може да е било използвано вече. Получете нова парола, за да подадете с тази заявка.**</span><span class="sxs-lookup"><span data-stu-id="730f2-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="730f2-113">Това съобщение означава, че трябва да изпълните инсталирането на конектора за сертификат като администратор.</span><span class="sxs-lookup"><span data-stu-id="730f2-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="730f2-114">В някои среди сървърите, където се изпълнява сертификатът за настройване, трябва да използват прокси сървър, за да се свързват с настройките, така че Конекторът на сертификата трябва да използва пълномощник.</span><span class="sxs-lookup"><span data-stu-id="730f2-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="730f2-115">В някои случаи Конекторът на NDES игнорира конфигурираните настройки на прокси сървър и може да е необходимо да конфигурирате настройките на прокси сървъра, докато се изпълнява в контекста на защитата на LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="730f2-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="730f2-116">Решението е да стартирате Internet Explorer като система и да конфигурирате прокси сървър в IE.</span><span class="sxs-lookup"><span data-stu-id="730f2-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="730f2-117">След рестартиране на услугата за конектори за NDES Конекторът за връзка се свързва с настройките.</span><span class="sxs-lookup"><span data-stu-id="730f2-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="730f2-118">**Потребителските устройства повече не получават сертификати за SCEP от NDES.**</span><span class="sxs-lookup"><span data-stu-id="730f2-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="730f2-119">Възможно е сертификатът за удостоверяване на клиент, издаден на сървъра за NDES, и определен по време на инсталирането на NDES Connector, да е изтекъл или липсва.</span><span class="sxs-lookup"><span data-stu-id="730f2-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="730f2-120">За да отстраните проблема:</span><span class="sxs-lookup"><span data-stu-id="730f2-120">To resolve:</span></span> 
 
1. <span data-ttu-id="730f2-121">Деинсталирайте конектора на NDES.</span><span class="sxs-lookup"><span data-stu-id="730f2-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="730f2-122">Използвайте тези данни, за да поискате ново удостоверяване на клиент или сертификат за удостоверяване на сървъра:</span><span class="sxs-lookup"><span data-stu-id="730f2-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="730f2-123">Име на тема: CN = външни FQDN</span><span class="sxs-lookup"><span data-stu-id="730f2-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="730f2-124">Алтернативно име на тема (и двете са задължителни): DNS = външни FQDN, DNS = вътрешно FQDN</span><span class="sxs-lookup"><span data-stu-id="730f2-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="730f2-125">Преинсталирайте NDES конектор с новия сертификат.</span><span class="sxs-lookup"><span data-stu-id="730f2-125">Reinstall the NDES connector with the new certificate.</span></span>