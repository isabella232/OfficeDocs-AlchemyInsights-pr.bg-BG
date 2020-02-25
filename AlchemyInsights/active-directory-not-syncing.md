---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265130"
---
# <a name="active-directory-not-syncing"></a>Active Directory не се синхронизира

Ако получавате грешки при синхронизацията, като например "няма скорошно синхронизиране" или забележите състоянието на синхронизиране на директории в портала за администриране на Office казва" последно синхронизирани преди повече от 3 дни," това може да е, че AADConnect има неправилни настройки или недостатъчно разрешения за извършване на синхронизация.  

Преинсталиране на AADConnect чрез бързи настройки може да реши проблема бързо:

1. [Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следвайте инструкциите за експресно инсталиране](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

За повече информация относно AADConnect сервизни акаунти вижте [Azure AD свързване: акаунти и разрешения](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
