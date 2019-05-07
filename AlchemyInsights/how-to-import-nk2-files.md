---
title: Как-към-внос-nk2-файлове
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: ed0c679cf3ed9d363e552c04a5ae6d0fc72f88dd
ms.sourcegitcommit: 6a229919cf67005e7e67841e9e45f2f3aa6833ef
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630005"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="ee730-102">Как да импортирате файлове с член .nk2</span><span class="sxs-lookup"><span data-stu-id="ee730-102">How to import .nk2 files</span></span> 

<span data-ttu-id="ee730-103">Когато стартирате Microsoft Outlook 2013, перспектива 2016, Outlook 2019 или Outlook за Office 365 за първи път, псевдоним кеш (съхраняват в файла *profilename*член .nk2) се импортира в скрито съобщение в хранилището ви по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="ee730-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="ee730-104">За да импортирате член .nk2 файлове в Outlook 2013, перспектива 2016, Outlook 2019 или Outlook за Office 365, се уверете, че член .nk2 файлът е в следната папка: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="ee730-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="ee730-105">**Забележка**: член .nk2 файлът трябва да има същото име като текущата си Outlook 2013 или Outlook 2016 профил.</span><span class="sxs-lookup"><span data-stu-id="ee730-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="ee730-106">По подразбиране името на профила е "Outlook".</span><span class="sxs-lookup"><span data-stu-id="ee730-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="ee730-107">За да проверите името на профил, изпълнете следните стъпки:</span><span class="sxs-lookup"><span data-stu-id="ee730-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="ee730-108">Щракнете върху **Старт**а след това щракнете върху **Контролен панел**.</span><span class="sxs-lookup"><span data-stu-id="ee730-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="ee730-109">Щракнете двукратно върху **поща**.</span><span class="sxs-lookup"><span data-stu-id="ee730-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="ee730-110">В диалоговия прозорец Настройка на поща изберете **Покажи профилите**.</span><span class="sxs-lookup"><span data-stu-id="ee730-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="ee730-111">Изберете **Старт** > **тичам**.</span><span class="sxs-lookup"><span data-stu-id="ee730-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="ee730-112">В полето **Отвори** въведете *outlook.exe /importnk2*и след това изберете **OK**.</span><span class="sxs-lookup"><span data-stu-id="ee730-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="ee730-113">След като импортирате определителен член .nk2 пила, съдържанието на файла се сливат в кеша на съществуващите псевдоним, съхранени във вашата пощенска кутия.</span><span class="sxs-lookup"><span data-stu-id="ee730-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="ee730-114">**Забележка**: член .nk2 файлът е преименуван с разширение .old следващия път, когато стартирате Outlook 2013, перспектива 2016, Outlook 2019 или Outlook за Office 365.</span><span class="sxs-lookup"><span data-stu-id="ee730-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365.</span></span> <span data-ttu-id="ee730-115">Ако искате да импортирате отново определителен член .nk2 пила, премествам .old разширение на файловото име пръв.</span><span class="sxs-lookup"><span data-stu-id="ee730-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="ee730-116">За повече информация вижте [Импортиране или копирате списъка автоматично довършване на друг компютър](https://support.microsoft.com/en-us/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="ee730-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/en-us/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>