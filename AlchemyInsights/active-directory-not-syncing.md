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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937090"
---
# <a name="active-directory-not-syncing"></a>Active Directory не се синхронизира

Ако получавате грешки при синхронизиране, като например "няма скорошно синхронизиране", или забележите състоянието на синхронизиране на справочен указател в портала за администриране на Office казва "Последно синхронизирано преди повече от 3 дни", може да се окаже, че AADConnect има неправилни настройки или недостатъчни разрешения за извършване на синхронизиране.  

Преинсталирането на AADConnect с помощта на експресни настройки може да реши проблема бързо:

1. [Изтеглете най-новата версия на AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Следвайте инструкциите за експресна инсталация](/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect трябва да се инсталира на Windows Server 2012 или по-нова версия. Този сървър трябва да бъде присъединен към домейн и може да бъде домейнов контролер или сървър член. За пълен списък на изискванията за Свързване и предварителните изисквания на Azure AD прегледайте Предварителни [изисквания за Azure AD Свързване.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

За повече информация относно акаунтите за услуги на AADConnect вж. [Azure AD Свързване: Акаунти и разрешения.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
