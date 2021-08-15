---
title: UPN синхронизирането е забранено
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: fc163fae4d348d7c7cf117bd457f999b42f96bec7c1eb9aa1435e346131d06de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038101"
---
# <a name="upn-sync-disabled"></a>UPN синхронизирането е забранено

Ако сте започнали да синхронизирате с Azure AD преди 30 март 2016 г., изпълнете следната кратка команда Azure AD PowerShell, за да разрешите UPN софтуерно съвпадение само за вашата организация:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UpN soft match се включва автоматично за организации, които са започнали синхронизиране с Azure AD на или след 30 март 2016 г.
  
За да научите повече за разрешаването на софтуерно съвпадение в UPN и други функции за синхронизиране, вж. [Azure AD Свързване на услугите за синхронизиране.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

