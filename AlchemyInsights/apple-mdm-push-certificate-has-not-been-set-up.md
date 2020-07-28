---
title: Apple MDM не е настроен push сертификат
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438761"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="1eea3-102">Apple MDM не е настроен push сертификат</span><span class="sxs-lookup"><span data-stu-id="1eea3-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="1eea3-103">Сертификат за натискане на Apple MDM (известен също като сертификат за известяване с натискане на Apple ( APNS) не е конфигуриран за вашия абонамент.</span><span class="sxs-lookup"><span data-stu-id="1eea3-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="1eea3-104">Без apple MDM Push сертификат конфигуриран, не можете да се регистрирате и управление на iOS и Mac OS устройства.</span><span class="sxs-lookup"><span data-stu-id="1eea3-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="1eea3-105">След като добавите сертификата intune, потребителите могат да инсталират приложението портал за компания да запишат своите iOS устройства.</span><span class="sxs-lookup"><span data-stu-id="1eea3-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="1eea3-106">Изберете **"Съгласен съм".**</span><span class="sxs-lookup"><span data-stu-id="1eea3-106">Select **"I agree."**</span></span> <span data-ttu-id="1eea3-107">да дадете разрешение на Microsoft да изпраща данни на Apple.</span><span class="sxs-lookup"><span data-stu-id="1eea3-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="1eea3-108">Изберете **Изтегляне на вашия CSR** заявка за подписване на сертификат Intune, необходим за създаване на Apple MDM push сертификат.</span><span class="sxs-lookup"><span data-stu-id="1eea3-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="1eea3-109">Файлът се използва за искане на сертификат за доверие връзка от Apple Натиснете сертификати портал.</span><span class="sxs-lookup"><span data-stu-id="1eea3-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="1eea3-110">Изберете **Създаване на MDM push сертификат,** за да отидете на портала за сертификати на Apple Push.</span><span class="sxs-lookup"><span data-stu-id="1eea3-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="1eea3-111">Влезте с вашия Apple ID на фирмата си, след което изберете **Създаване на сертификат**.</span><span class="sxs-lookup"><span data-stu-id="1eea3-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="1eea3-112">Изберете **Избор на файл**, намерете файла заявка за подписване на сертификат, след което изберете **Качване**.</span><span class="sxs-lookup"><span data-stu-id="1eea3-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="1eea3-113">На страницата потвърждение изберете **Изтегляне,** за да изтеглите файла сертификат (.pem) и запишете файла локално.</span><span class="sxs-lookup"><span data-stu-id="1eea3-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="1eea3-114">**Забележка**: Сертификатът е свързан с Apple ID, използван за създаването му.</span><span class="sxs-lookup"><span data-stu-id="1eea3-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="1eea3-115">Като най-добра практика използвайте apple ID на фирма за задачи за управление и се уверете, че пощенската кутия се следи от повече от едно лице или чрез списък за разпространение.</span><span class="sxs-lookup"><span data-stu-id="1eea3-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="1eea3-116">Никога не използвайте лична Apple ID.</span><span class="sxs-lookup"><span data-stu-id="1eea3-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="1eea3-117">Използвайте същия идентификационен номер на Apple, за да подновите сертификата на Apple Push на всеки 12 месеца.</span><span class="sxs-lookup"><span data-stu-id="1eea3-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="1eea3-118">Въведете идентификационния номер на Apple, използван за създаване на вашия Apple MDM сертификат за push.</span><span class="sxs-lookup"><span data-stu-id="1eea3-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="1eea3-119">Запишете този ИД като напомняне за това, кога трябва да подновите сертификата.</span><span class="sxs-lookup"><span data-stu-id="1eea3-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="1eea3-120">Отидете на сертификата (.pem) файл, изберете **Отваряне**и след това изберете **Качване**.</span><span class="sxs-lookup"><span data-stu-id="1eea3-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="1eea3-121">С push сертификата, Intune може да се регистрирате и да управлявате Apple устройства.</span><span class="sxs-lookup"><span data-stu-id="1eea3-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>