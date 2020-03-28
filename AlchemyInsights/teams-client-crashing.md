---
title: Клиент на Teams има проблем със срив?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030516"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a6d68-102">Клиент на Teams има проблем със срив?</span><span class="sxs-lookup"><span data-stu-id="a6d68-102">Teams client crashing?</span></span>

<span data-ttu-id="a6d68-103">Ако клиентът ви в Teams има проблем със срив, опитайте следното:</span><span class="sxs-lookup"><span data-stu-id="a6d68-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a6d68-104">Ако използвате настолното приложение Teams, [уверете се, че приложението е напълно актуализирано](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a6d68-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a6d68-105">Уверете се, че всички [URL и диапазони от адреси за Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) са достъпни.</span><span class="sxs-lookup"><span data-stu-id="a6d68-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a6d68-106">Влезте със своя акаунт на администратор и проверете [вашето табло за изправност на услугите](https://docs.microsoft.com/office365/enterprise/view-service-health), за да проверите дали няма прекъсване или влошаване на услугата.</span><span class="sxs-lookup"><span data-stu-id="a6d68-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="a6d68-107">Като последна стъпка можете да се опитате да изчистите кеша на вашия клиент в Teams:</span><span class="sxs-lookup"><span data-stu-id="a6d68-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="a6d68-108">Напълно излезте от настолния клиент на Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a6d68-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="a6d68-109">Можете да щракнете с десния бутон на мишката върху **Teams** от иконата в системната област и да щракнете върху **Изход**, или да изпълнете диспечера на задачите, за да прекратите напълно процеса.</span><span class="sxs-lookup"><span data-stu-id="a6d68-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="a6d68-110">Отидете на File Explorer и въведете %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="a6d68-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="a6d68-111">След като влезете в справочния указател, ще видите няколко от следните папки:</span><span class="sxs-lookup"><span data-stu-id="a6d68-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="a6d68-112">От **Кеш за приложенията**, отидете на Кеш и изтрийте всеки от файловете в местоположението на кеша: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="a6d68-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="a6d68-113">От **Blob_storage**, изтрийте всички файлове: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="a6d68-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="a6d68-114">От **Blob_storage**, изтрийте всички файлове: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="a6d68-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="a6d68-115">От **Бази данни**, изтрийте всички файлове: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="a6d68-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="a6d68-116">От **GPUCache**, изтрийте всички файлове: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="a6d68-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="a6d68-117">От **IndexedDB**, изтрийте файла .db: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="a6d68-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="a6d68-118">От **Локално място за съхранение**, изтрийте всички файлове: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="a6d68-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="a6d68-119">И накрая, от **tmp**, изтрийте всеки файл: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="a6d68-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="a6d68-120">Рестартирайте своя клиент в Teams.</span><span class="sxs-lookup"><span data-stu-id="a6d68-120">Restart your Teams client.</span></span>
