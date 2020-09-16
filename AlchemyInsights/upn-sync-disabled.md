---
title: UPN синхронизирането е забранено
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749503"
---
# <a name="upn-sync-disabled"></a>UPN синхронизирането е забранено

Ако сте стартирали синхронизирането на Azure AD преди 30 март 2016, изпълнете следната кратка команда на Azure AD PowerShell, за да разрешите UPN меко съвпадение само за вашата организация:
  
 **Set-MsolDirSyncFeature-функция EnableSoftMatchOnUpn-Enable $True**
  
UPN Soft Match се включва автоматично за организации, които са започнали да се синхронизират с Azure AD на или след 30 март, 2016.
  
За да научите повече за разрешаването на плавно съвпадение по UPN и други функции за синхронизиране, вижте [функции за услугата за синхронизиране на AZURE ad Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

