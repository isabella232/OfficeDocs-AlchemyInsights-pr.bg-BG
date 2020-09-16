---
title: Не е настроен сертификат на Apple MDM Push
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716846"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="278be-102">Не е настроен сертификат на Apple MDM Push</span><span class="sxs-lookup"><span data-stu-id="278be-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="278be-103">Сертификат на Apple MDM Push (известен също като сертификат за услуга за насочени известия за Apple) не е конфигуриран за абонамента ви.</span><span class="sxs-lookup"><span data-stu-id="278be-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="278be-104">Без конфигуриран сертификат на Apple MDM Push, не можете да задавате и управлявате устройства с iOS и Mac OS.</span><span class="sxs-lookup"><span data-stu-id="278be-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="278be-105">След като добавите сертификат за включване, потребителите могат да инсталират приложението Company Portal, за да запишат своите устройства с iOS.</span><span class="sxs-lookup"><span data-stu-id="278be-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="278be-106">Изберете **"Съгласен съм".**</span><span class="sxs-lookup"><span data-stu-id="278be-106">Select **"I agree."**</span></span> <span data-ttu-id="278be-107">за да дадете на Microsoft разрешение за изпращане на данни на Apple.</span><span class="sxs-lookup"><span data-stu-id="278be-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="278be-108">Изберете **изтегляне на вашия CSR** командата за подписване на сертификат, която се изисква, за да създадете сертификат на Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="278be-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="278be-109">Файлът се използва, за да поискате сертификат за надеждност на връзката от портала за насочени сертификати на Apple.</span><span class="sxs-lookup"><span data-stu-id="278be-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="278be-110">Изберете **Създаване на вашия сертификат за MDM Push** , за да отидете на портала за насочени сертификати на Apple.</span><span class="sxs-lookup"><span data-stu-id="278be-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="278be-111">Влезте със своя служебен ИД на Apple и след това изберете **Създаване на сертификат**.</span><span class="sxs-lookup"><span data-stu-id="278be-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="278be-112">Изберете **избор на файл**, намерете файла на искането за подписване на сертификат и след това изберете **качване**.</span><span class="sxs-lookup"><span data-stu-id="278be-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="278be-113">На страницата за потвърждение изберете **изтегляне** , за да изтеглите файла на сертификата (. pem), и запишете файла локално.</span><span class="sxs-lookup"><span data-stu-id="278be-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="278be-114">**Забележка**: сертификатът е СВЪРЗАН с ИД на Apple, използван за създаването му.</span><span class="sxs-lookup"><span data-stu-id="278be-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="278be-115">Като най-добра практика Използвайте фирмен ИД на Apple за управление на задачи и се уверете, че пощенската кутия е наблюдавана от повече от един човек или с помощта на списък за разпространение.</span><span class="sxs-lookup"><span data-stu-id="278be-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="278be-116">Никога не използвайте личен ИД за Apple.</span><span class="sxs-lookup"><span data-stu-id="278be-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="278be-117">Използвайте един и същ ИД на Apple, за да подновите натиснатия сертификат на Apple на всеки 12 месеца.</span><span class="sxs-lookup"><span data-stu-id="278be-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="278be-118">Въведете ИДЕНТИФИКАТОРа на Apple, използван за създаване на вашия сертификат за Push на Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="278be-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="278be-119">Запишете това име като напомняне, когато трябва да подновите сертификата.</span><span class="sxs-lookup"><span data-stu-id="278be-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="278be-120">Отидете на файла сертификат (. pem), изберете **Отвори**и след това изберете **качване**.</span><span class="sxs-lookup"><span data-stu-id="278be-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="278be-121">Чрез Push сертификат, функцията за записване може да записва и управлява устройства на Apple.</span><span class="sxs-lookup"><span data-stu-id="278be-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>