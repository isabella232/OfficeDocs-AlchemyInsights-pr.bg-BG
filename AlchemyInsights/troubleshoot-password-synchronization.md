---
title: Отстраняване на неизправности при синхронизиране на пароли
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387866"
---
# <a name="troubleshoot-password-synchronization"></a>Отстраняване на неизправности при синхронизиране на пароли

За отстраняване на проблеми при синхронизиране на пароли, стартирайте с помощта на тази задача за отстраняване на неизправности СД свързване, за да определите защо паролите не се синхронизират. За да започнете, отидете [на Управление на директно синхронизиране](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Отворете нова сесия на Windows PowerShell на вашия сървър Azure AD свързване и изберете опцията **Изпълни като администратор** .

2. Изпълнение на набор за изпълнение RemoteSigned или Set-ExecutionPolicy Неограничен.

3. Стартирайте съветника за Azure AD свързване.

4. Отидете на страницата Допълнителни задачи > **Отстраняване на неизправности**  >  **.**

5. Изберете **Стартиране,** за да отворите менюто за отстраняване на неизправности на PowerShell.

6. Изберете **Отстраняване на неизправности при синхронизиране на пароли**.

    Проблемът обикновено е, че паролата не се синхронизира за определен потребителски акаунт.

    **Бележки** Синхронизиране на пароли е неуспешно, ако последната успешно синхронизиране на паролата е преди известно време.

За повече помощ за отстраняване на синхронизацията на пароли вижте [Отстраняване на синхронизиране на пароли хеш с Azure AD Свързване sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).