---
title: UPN синхронизация с увреждания
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532320"
---
# <a name="upn-sync-disabled"></a>UPN синхронизация с увреждания

Ако сте започнали syncing към лазурно АД преди 30 март 2016, изпълнете следните Azure АД PowerShell cmdlet да разрешите UPN мек мач за вашата организация само:
  
 **Комплект-MsolDirSyncFeature-функция EnableSoftMatchOnUpn-давам възможност на $True**
  
UPN мек мач е включено автоматично за организации, които започнали syncing към лазурните реклама на или след 30 март 2016 г.
  
За да научите повече за активирането на мек мач на UPN и други функции за синхронизиране, моля вижте [Azure АД свържете синхронизация услуга функции](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

