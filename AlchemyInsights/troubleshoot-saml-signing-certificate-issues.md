---
title: Отстраняване на проблеми със сертификатите за SAML подписване
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692524"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="99eec-102">Отстраняване на проблеми със сертификатите за SAML подписване</span><span class="sxs-lookup"><span data-stu-id="99eec-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="99eec-103">За да отстраните проблема със сертификат за подписване на SAML, изпълнете следните Препоръчителни стъпки:</span><span class="sxs-lookup"><span data-stu-id="99eec-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="99eec-104">Когато добавите корпоративна програма, която поддържа SSO, Azure ще генерира сертификат, наречен сертификат за подписване на [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span><span class="sxs-lookup"><span data-stu-id="99eec-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="99eec-105">Този сертификат има дата на изтичане на срока от 3 години.</span><span class="sxs-lookup"><span data-stu-id="99eec-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="99eec-106">За да промените датата на изтичане на срока на вашия сертификат, вижте [Персонализиране на срока на валидност на сертификата на федерацията и прехвърлянето му към нов сертификат](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="99eec-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="99eec-107">Azure ще използва този сертификат, за да подписва SAML жетони, поискани от приложението и да го изпрати към приложението за успешно SSO.</span><span class="sxs-lookup"><span data-stu-id="99eec-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="99eec-108">За да завърши това, изтеглете сертификата от портала на Azure и го изпратете до производителя на приложението, за да завършите процеса на SSO.</span><span class="sxs-lookup"><span data-stu-id="99eec-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="99eec-109">След като този процес приключи, вашата кандидатура ще се довери на този сертификат и всички SAML маркери, подписани от този сертификат, ще бъдат приети от приложението.</span><span class="sxs-lookup"><span data-stu-id="99eec-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="99eec-110">Ако този сертификат изтече, създайте нов сертификат, актуализирайте го на доставчика на приложението и след това го направете активен в Azure.</span><span class="sxs-lookup"><span data-stu-id="99eec-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="99eec-111">За повече информация вижте [подновяване на сертификат, който скоро ще изтече](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="99eec-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="99eec-112">Ако сертификатът изтече, потребителят няма да бъде блокиран.</span><span class="sxs-lookup"><span data-stu-id="99eec-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="99eec-113">[Добавете имейл адрес за уведомленията](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) , които трябва да бъдат получени, преди да изтече текущият сертификат.</span><span class="sxs-lookup"><span data-stu-id="99eec-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="99eec-114">Step-4 е незадължителен.</span><span class="sxs-lookup"><span data-stu-id="99eec-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="99eec-115">Промяна на опциите за подписване на приложението SAML сертификат и алгоритъм за подписване на сертификат.</span><span class="sxs-lookup"><span data-stu-id="99eec-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="99eec-116">За повече информация вижте [Промяна на опциите за подписване на сертификат и алгоритъм за подписване](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="99eec-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

