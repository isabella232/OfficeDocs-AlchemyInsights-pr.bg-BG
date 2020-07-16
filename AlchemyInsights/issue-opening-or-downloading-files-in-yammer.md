---
title: Проблем при отваряне или изтегляне на файлове в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148185"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="57dca-102">Проблем при отваряне или изтегляне на файлове в Yammer</span><span class="sxs-lookup"><span data-stu-id="57dca-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="57dca-103">Класически Yammer поддържа няколко варианта за качване на файлове в съобщения и групи.</span><span class="sxs-lookup"><span data-stu-id="57dca-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="57dca-104">В зависимост от мрежовата конфигурация файловете по подразбиране за съхранение в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57dca-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="57dca-105">Избор на файл в новия Yammer все още не поддържа всички опции, налични в класическия Yammer.</span><span class="sxs-lookup"><span data-stu-id="57dca-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="57dca-106">Бъдещата актуализация ще добави допълнителни функции.</span><span class="sxs-lookup"><span data-stu-id="57dca-106">A future update will add additional features.</span></span> <span data-ttu-id="57dca-107">За повече информация вижте [Прикачване на файл или изображение към разговор публикация на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="57dca-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="57dca-108">**Не може да се отвори или изтегли файл**</span><span class="sxs-lookup"><span data-stu-id="57dca-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="57dca-109">Файлът може да качите в Yammer, но също така да се свързвате към файл в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="57dca-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="57dca-110">За да отстраните проблема, първо трябва да определите местоположението на файла.</span><span class="sxs-lookup"><span data-stu-id="57dca-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="57dca-111">Ако файлът е качен в Yammer, той ще има \*.yammer.com URL.</span><span class="sxs-lookup"><span data-stu-id="57dca-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="57dca-112">Уверете се, че задължителните URL адреси и IP адреси са отблокирани.</span><span class="sxs-lookup"><span data-stu-id="57dca-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="57dca-113">За повече информация вижте публикацията [в блога с помощта на твърди кодирани IP адреси за Yammer не се препоръчва](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="57dca-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="57dca-114">Проверете дали потребител, който също е глобален администратор може да изтегли файла.</span><span class="sxs-lookup"><span data-stu-id="57dca-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="57dca-115">Ако файлът е поверително, може да се наложи да използвате режим на лично съдържание.</span><span class="sxs-lookup"><span data-stu-id="57dca-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="57dca-116">За повече информация вижте [след монитор частно съдържание в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="57dca-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="57dca-117">**Yammer гости и файлове на ниво мрежа в SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="57dca-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="57dca-118">[Ниво на мрежата гости в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не използват Azure AD B2B и са вътрешни за услугата Yammer, така че те нямат достъп до Yammer файлове, съхранени в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57dca-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="57dca-119">Създаване на външен AAD B2B потребител, който има достъп до библиотеки с документи в SharePoint Online с помощта на тази самоличност.</span><span class="sxs-lookup"><span data-stu-id="57dca-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="57dca-120">За информация относно бъдещите Azure AD B2B гост поддръжка в Yammer вижте [Business-to-business (B2B) гост поддръжка в Yammer преглед - условия за клиенти и често задавани въпроси](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="57dca-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>