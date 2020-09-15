---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697618"
---
# <a name="active-directory-not-syncing"></a>Active Directory не се синхронизира

Ако получавате грешки при синхронизиране, като например "няма Последни синхронизации" или Забележка състоянието на синхронизиране на справочен указател в портала за администратори на Office казва "Последно синхронизиране повече от 3 дни назад", може да се окаже, че AADConnect има грешни настройки или недостатъчни разрешения за извършване на синхронизиране.  

Преинсталирането на AADConnect с помощта на експресните настройки може бързо да отстрани проблема:

1. [Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следвайте инструкциите за експресната инсталация](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

За повече информация за акаунтите за AADConnect Services вижте [AZURE ad Connect: акаунти и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
