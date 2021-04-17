---
title: Active Directory не се синхронизира
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822840"
---
# <a name="active-directory-not-syncing"></a>Active Directory не се синхронизира

Ако получавате грешки при синхронизиране, като например "няма скорошно синхронизиране", или забележите състоянието на синхронизиране на справочен указател в портала за администриране на Office, "Последно синхронизирано преди повече от 3 дни", може да се окаже, че AADConnect има неправилни настройки или недостатъчни разрешения за извършване на синхронизиране.  

Преинсталирането на AADConnect с помощта на експресни настройки може да реши проблема бързо:

1. [Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следвайте инструкциите за експресна инсталация](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

За повече информация относно акаунтите за услуги на AADConnect вижте [Azure AD Connect: Акаунти и разрешения.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
