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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889207"
---
# <a name="active-directory-not-syncing"></a>Active Directory не се синхронизира

Ако получавате грешки при синхронизиране, като например "няма скорошно синхронизиране", или забележите състоянието на синхронизиране на справочен указател в портала за администриране на Office, казва "Последно синхронизирано преди повече от 3 дни", може да се окаже, че AADConnect има неправилни настройки или недостатъчни разрешения за извършване на синхронизиране.  

Преинсталирането на AADConnect с помощта на експресни настройки може да реши проблема бързо:

1. [Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следвайте инструкциите за експресна инсталация](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect трябва да се инсталира на Windows Server 2012 или по-нова версия. Този сървър трябва да бъде присъединен към домейн и може да бъде домейнов контролер или сървър член. За пълен списък на изискванията и предварителните изисквания Свързване Azure AD прегледайте Предварителни [изисквания за Azure AD Свързване.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

За повече информация относно акаунтите за услуги на AADConnect вижте [Azure AD Свързване: Акаунти и разрешения.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
