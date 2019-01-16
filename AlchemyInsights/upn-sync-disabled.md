---
title: UPN синхронизация с увреждания
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276675"
---
# <a name="upn-sync-disabled"></a>UPN синхронизация с увреждания

Ако сте започнали syncing към лазурно АД преди 30 март 2016, изпълнете следните Azure АД PowerShell cmdlet да разрешите UPN мек мач за вашата организация само:
  
 **Комплект-MsolDirSyncFeature-функция EnableSoftMatchOnUpn-давам възможност на $True**
  
UPN мек мач е включено автоматично за организации, които започнали syncing към лазурните реклама на или след 30 март 2016 г.
  
За да научите повече за активирането на мек мач на UPN и други функции за синхронизиране, моля вижте [Azure АД свържете синхронизация услуга функции](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

