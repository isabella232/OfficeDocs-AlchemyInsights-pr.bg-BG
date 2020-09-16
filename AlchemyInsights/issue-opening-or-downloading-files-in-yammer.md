---
title: Проблем при отварянето или изтеглянето на файлове в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695638"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="d1d86-102">Проблем при отварянето или изтеглянето на файлове в Yammer</span><span class="sxs-lookup"><span data-stu-id="d1d86-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="d1d86-103">Класическата Yammer поддържа множество опции за качване на файлове в съобщения и групи.</span><span class="sxs-lookup"><span data-stu-id="d1d86-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="d1d86-104">В зависимост от конфигурацията на мрежата, файлове по подразбиране за място за съхранение в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1d86-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="d1d86-105">Опцията за избор на файл в нови Yammer все още не поддържа всички опции, които са налични в класическата Yammer.</span><span class="sxs-lookup"><span data-stu-id="d1d86-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="d1d86-106">Бъдеща актуализация ще добави допълнителни функции.</span><span class="sxs-lookup"><span data-stu-id="d1d86-106">A future update will add additional features.</span></span> <span data-ttu-id="d1d86-107">За повече информация вижте [Прикачване на файл или изображение към публикация в разговор на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="d1d86-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="d1d86-108">**Не можете да отворите или изтеглите файл**</span><span class="sxs-lookup"><span data-stu-id="d1d86-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="d1d86-109">Даден файл може да се качи в Yammer, но също така да се свързва към файл в SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="d1d86-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="d1d86-110">За да отстраните проблема, първо трябва да определите местоположението на файла.</span><span class="sxs-lookup"><span data-stu-id="d1d86-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="d1d86-111">Ако файлът е качен в Yammer, той ще има URL адрес \*. yammer.com.</span><span class="sxs-lookup"><span data-stu-id="d1d86-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="d1d86-112">Уверете се, че изискваните URL адреси и IP адреси са Разблокирани.</span><span class="sxs-lookup"><span data-stu-id="d1d86-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="d1d86-113">За повече информация вижте публикацията в блог [с помощта на ТРУДНИ IP адреси за Yammer не се препоръчва](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="d1d86-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="d1d86-114">Проверете дали потребител, който е и глобален администратор, може да Изтегли файла.</span><span class="sxs-lookup"><span data-stu-id="d1d86-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="d1d86-115">Ако файлът е личен, е възможно да се наложи да използвате частното съдържание.</span><span class="sxs-lookup"><span data-stu-id="d1d86-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="d1d86-116">За повече информация вижте [наблюдение на личното съдържание в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="d1d86-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="d1d86-117">**Клиенти и файлове в мрежата на Yammer в SharePoint online**</span><span class="sxs-lookup"><span data-stu-id="d1d86-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="d1d86-118">[Гостите на ниво мрежа в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не използват AZURE ad B2B и са вътрешни за услугата yammer, така че да не могат да имат достъп до файлове на yammer, съхранени в SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d1d86-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="d1d86-119">Създаване на външен потребител на потребителски интерфейс, който има достъп до библиотеките с документи в SharePoint Online, с помощта на тази самоличност.</span><span class="sxs-lookup"><span data-stu-id="d1d86-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="d1d86-120">За информация относно бъдещия поддръжка на Azure AD B2B за гости в Yammer вижте [поддръжка за гост на фирма за бизнес (B2B) в предварителния преглед на Yammer – общи условия и ЧЗВ за клиенти](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="d1d86-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>