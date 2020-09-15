---
title: Отстраняване на неизправности при синхронизиране на парола
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
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664915"
---
# <a name="troubleshoot-password-synchronization"></a>Отстраняване на неизправности при синхронизиране на парола

За отстраняване на проблеми при синхронизиране на парола започнете с помощта на тази задача за отстраняване на неизправности с "пад", за да определите защо паролите не се синхронизират. За да започнете, отидете на [управление на директното синхронизиране](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Отворете нова сесия на Windows PowerShell на вашия сървър на Azure AD Connect и изберете опцията **Изпълнявай като администратор** .

2. Run Set-ExecutionPolicy RemoteSigned или Set-ExecutionPolicy неограничени.

3. Стартирайте съветника за свързване на Azure AD.

4. Отиване на страницата с допълнителни задачи > **отстраняване на неизправности**  >  **след**това.

5. Изберете **стартиране** , за да отворите менюто отстраняване на неизправности на PowerShell.

6. Изберете **отстраняване на неизправности при синхронизиране на парола**.

    Обикновено проблемът е, че една парола не е синхронизирана за конкретен потребителски акаунт.

    **Бележки** Синхронизирането на парола е неуспешно, ако последното успешно синхронизиране на парола е било преди известно време.

За повече помощ за отстраняване на неизправности при синхронизиране на парола вижте [отстраняване на неизправности при хеширане с криптиране чрез AZURE ad Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).