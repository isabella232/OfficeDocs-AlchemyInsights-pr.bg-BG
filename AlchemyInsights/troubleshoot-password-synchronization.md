---
title: Отстраняване на неизправности при синхронизиране на пароли
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
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105737"
---
# <a name="troubleshoot-password-synchronization"></a>Отстраняване на неизправности при синхронизиране на пароли

За да отстраните проблеми със синхронизирането на пароли, започнете с помощта на Свързване за отстраняване на неизправности, за да определите защо паролите не се синхронизират. За да започнете, отидете на [Управление на директно синхронизиране](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Отворете нова сесия Windows PowerShell azure AD Свързване и изберете опцията Изпълни **като** администратор.

2. Изпълнявайте Set-ExecutionPolicy с отдалечен подпис или Set-ExecutionPolicy неограничени.

3. Стартирайте съветника за Свързване Azure AD.

4. Отидете на страницата Допълнителни задачи > **Отстраняване на неизправности**  >  **напред**.

5. Изберете **Стартиране, за** да отворите менюто за отстраняване на неизправности на PowerShell.

6. Изберете **Отстраняване на неизправности при синхронизиране на пароли**.

    Проблемът обикновено е, че паролата не се синхронизира за конкретен потребителски акаунт.

    **Бележки** Синхронизирането на пароли е неуспешно, ако последното успешно синхронизиране на пароли е било преди известно време.

За повече помощ при отстраняване на неизправности при синхронизиране на пароли вижте Отстраняване на неизправности при синхронизиране на [хашта](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)на пароли с Azure AD Свързване синхронизиране.