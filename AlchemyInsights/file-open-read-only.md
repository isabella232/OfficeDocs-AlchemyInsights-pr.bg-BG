---
title: Отваряне на файл само за четене
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813173"
---
# <a name="file-open-read-only"></a><span data-ttu-id="70556-102">Отваряне на файл само за четене</span><span class="sxs-lookup"><span data-stu-id="70556-102">File open read-only</span></span>

<span data-ttu-id="70556-103">Може да откриете, че когато отваряте файлове, те се отварят само за четене.</span><span class="sxs-lookup"><span data-stu-id="70556-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="70556-104">В някои случаи това е за допълнителна защита, например когато отваряте файлове от интернет, а други случаи това може да се дължи на настройка, която може да бъде променена.</span><span class="sxs-lookup"><span data-stu-id="70556-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="70556-105">Ето някои сценарии, при които файлът се отваря само за четене, и някои стъпки, които можете да предприемете, за да промените това.</span><span class="sxs-lookup"><span data-stu-id="70556-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="70556-106">**Моята антивирусна програма ги кара да отварят само за четене**</span><span class="sxs-lookup"><span data-stu-id="70556-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="70556-107">Някои антивирусни програми може да ви предпазят от потенциално опасни файлове, като ги отварят само за четене.</span><span class="sxs-lookup"><span data-stu-id="70556-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="70556-108">Може да се наложи да се консултирате с вашия доставчик на антивирусна програма, за да научите как да регулирате тези настройки.</span><span class="sxs-lookup"><span data-stu-id="70556-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="70556-109">BitDefender например има съдържание за добавяне на изключения на приложения тук: Как да добавите изключения на приложения или процеси в [центъра за управление на Bitdefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="70556-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="70556-110">**Зададени ли са свойствата на файла само за четене?**</span><span class="sxs-lookup"><span data-stu-id="70556-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="70556-111">Можете да проверите свойствата на файла, като щракнете с десния бутон върху файла и изберете Свойства.</span><span class="sxs-lookup"><span data-stu-id="70556-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="70556-112">Ако атрибутът само за четене е отметнат, можете да го премахнете от отметката и да щракнете върху OK.</span><span class="sxs-lookup"><span data-stu-id="70556-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="70556-113">**Съдържанието е в защитен изглед**</span><span class="sxs-lookup"><span data-stu-id="70556-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="70556-114">Файловете от интернет и от други потенциално опасни местоположения могат да съдържат вируси, червеи или други видове злонамерен софтуер, които могат да навредят на компютъра ви.</span><span class="sxs-lookup"><span data-stu-id="70556-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="70556-115">Това обикновено се отнася и за прикачените файлове към имейла или файловете, които сте изтеглили.</span><span class="sxs-lookup"><span data-stu-id="70556-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="70556-116">За да защитите компютъра си, файловете от тези потенциално опасни местоположения се отварят в защитен изглед.</span><span class="sxs-lookup"><span data-stu-id="70556-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="70556-117">С помощта на защитен изглед можете да прочетете файл и да видите съдържанието му, като същевременно намалите рисковете.</span><span class="sxs-lookup"><span data-stu-id="70556-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="70556-118">За повече информация относно защитения изглед и как да промените настройките вижте тази статия: [Какво представлява защитеният изглед?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="70556-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="70556-119">**OneDrive пълен ли е?**</span><span class="sxs-lookup"><span data-stu-id="70556-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="70556-120">Ако файлът се съхранява в OneDrive и мястото за съхранение в OneDrive е пълно, няма да можете да запишете документа, докато не сте под определеното място.</span><span class="sxs-lookup"><span data-stu-id="70556-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="70556-121">Можете да проверите свободното си място в OneDrive, като щракнете върху иконата на OneDrive в центъра за известия и изберете Управление на мястото за съхранение или можете да отидете в , да влезете и да обърнете внимание на количеството използвано място [https://onedrive.live.com](https://onedrive.live.com) в долния ляв ъгъл на екрана.</span><span class="sxs-lookup"><span data-stu-id="70556-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="70556-122">**Office активира ли се?**</span><span class="sxs-lookup"><span data-stu-id="70556-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="70556-123">Ако Office не е активиран или абонаментът ви е изтекъл, може да сте в режим на намалена функционалност само за четене.</span><span class="sxs-lookup"><span data-stu-id="70556-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="70556-124">За информация как да активирате Office вижте: Грешки при нелицензиран продукт [и активиране в Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="70556-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="70556-125">**Ако всичко друго е неуспешно...**</span><span class="sxs-lookup"><span data-stu-id="70556-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="70556-126">Опитайте да рестартирате компютъра</span><span class="sxs-lookup"><span data-stu-id="70556-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="70556-127">Инсталиране на актуализации на Office</span><span class="sxs-lookup"><span data-stu-id="70556-127">Install Office updates</span></span>
    
- <span data-ttu-id="70556-128">Извършване на онлайн поправка на Office</span><span class="sxs-lookup"><span data-stu-id="70556-128">Perform an Online repair of Office</span></span>
    

