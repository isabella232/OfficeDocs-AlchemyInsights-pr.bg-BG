---
title: Файлът е отворен само за четене
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745561"
---
# <a name="file-open-read-only"></a><span data-ttu-id="c4742-102">Файлът е отворен само за четене</span><span class="sxs-lookup"><span data-stu-id="c4742-102">File open read-only</span></span>

<span data-ttu-id="c4742-103">Можете да откриете, че когато отваряте файлове, те се отварят само за четене.</span><span class="sxs-lookup"><span data-stu-id="c4742-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="c4742-104">В някои случаи това е за допълнителна защита, като например когато отваряте файлове от интернет и други времена, това може да се дължи на настройка, която може да бъде променена.</span><span class="sxs-lookup"><span data-stu-id="c4742-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="c4742-105">Ето някои сценарии, при които даден файл отваря само за четене и някои стъпки, които можете да предприемете, за да промените това.</span><span class="sxs-lookup"><span data-stu-id="c4742-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="c4742-106">**Моята антивирусна програма е причината да се отварят само за четене**</span><span class="sxs-lookup"><span data-stu-id="c4742-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="c4742-107">Някои антивирусни програми могат да ви предпазят от потенциално опасни файлове, като ги отворите само за четене.</span><span class="sxs-lookup"><span data-stu-id="c4742-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="c4742-108">Може да се наложи да се консултирате с вашия доставчик на антивирусен софтуер, за да научите как да регулирате тези настройки.</span><span class="sxs-lookup"><span data-stu-id="c4742-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="c4742-109">BitDefender например има съдържание за добавяне на изключвания на приложения тук: [как да добавяте приложения или изключвания на процеси в BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="c4742-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="c4742-110">**Свойствата на файла зададени ли са само за четене?**</span><span class="sxs-lookup"><span data-stu-id="c4742-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="c4742-111">Можете да проверите свойствата на файла, като щракнете с десния бутон върху файла и изберете свойства.</span><span class="sxs-lookup"><span data-stu-id="c4742-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="c4742-112">Ако е отметнат атрибутът само за четене, можете да махнете отметката от него и да щракнете върху OK.</span><span class="sxs-lookup"><span data-stu-id="c4742-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="c4742-113">**Съдържанието е в защитен изглед**</span><span class="sxs-lookup"><span data-stu-id="c4742-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="c4742-114">Файлове от интернет и от други потенциално опасни местоположения може да съдържат вируси, червеи или други видове злонамерен софтуер, които могат да увредят компютъра ви.</span><span class="sxs-lookup"><span data-stu-id="c4742-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="c4742-115">Това обикновено е случаят с прикачените файлове или файловете, които сте изтеглили.</span><span class="sxs-lookup"><span data-stu-id="c4742-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="c4742-116">За да защитите компютъра си, файловете от тези потенциално опасни местоположения се отварят в защитен изглед.</span><span class="sxs-lookup"><span data-stu-id="c4742-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="c4742-117">Като използвате защитен изглед, можете да прочетете даден файл и да видите съдържанието му, като същевременно намалите рисковете.</span><span class="sxs-lookup"><span data-stu-id="c4742-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="c4742-118">За повече информация относно защитения изглед и как да промените настройките вижте тази статия: [Какво е защитен изглед?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="c4742-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="c4742-119">**Пълен ли е OneDrive?**</span><span class="sxs-lookup"><span data-stu-id="c4742-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="c4742-120">Ако файлът е съхранен в OneDrive и свободното място за съхранение в OneDrive е пълно, няма да можете да запишете документа, докато не се намирате под разпределения ви интервал.</span><span class="sxs-lookup"><span data-stu-id="c4742-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="c4742-121">Можете да проверите свободното си място в OneDrive, като щракнете върху иконата на OneDrive в центъра за известия и изберете управление на мястото за съхранение, или можете да отидете на [https://onedrive.live.com](https://onedrive.live.com) , влезте и отбележете размера на използваното място в долния ляв ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="c4742-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="c4742-122">**Активиран ли е Office?**</span><span class="sxs-lookup"><span data-stu-id="c4742-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="c4742-123">Ако Office не е активиран или ако абонаментът ви е изтекъл, можете да сте в режим на намалена функционалност "само за четене".</span><span class="sxs-lookup"><span data-stu-id="c4742-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="c4742-124">За информация как да активирате Office, вижте: [нелицензиран продукт и грешки при активиране в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="c4742-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="c4742-125">**Ако нищо друго не помогне...**</span><span class="sxs-lookup"><span data-stu-id="c4742-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="c4742-126">Опитайте да рестартирате компютъра</span><span class="sxs-lookup"><span data-stu-id="c4742-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="c4742-127">Инсталиране на актуализации на Office</span><span class="sxs-lookup"><span data-stu-id="c4742-127">Install Office updates</span></span>
    
- <span data-ttu-id="c4742-128">Изпълнение на онлайн поправка на Office</span><span class="sxs-lookup"><span data-stu-id="c4742-128">Perform an Online repair of Office</span></span>
    

