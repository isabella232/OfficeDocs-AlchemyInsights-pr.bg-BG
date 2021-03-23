---
title: Импортиране и експортиране от Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034918"
---
# <a name="import-and-export-from-yammer"></a>Импортиране и експортиране от Yammer

**Импортиране**

Опциите за импортиране на потребители са различни в зависимост от това дали вашата мрежа на Yammer е в [основен режим за Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), или не.

- **Non-Native режим**: потребителите могат да бъдат импортирани в групи с помощта на " [Добавяне от адресната книга](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) " (лимит към потребители на 100) в настройките на група или в мрежата чрез [групово актуализиране](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) в Network Admin.
- **Native Mode**: членството в група и операцията за членство в мрежата трябва да се извършва от [портала за администриране на Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users), [портала на Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)или чрез друга опция за Azure ad. Мрежите в основен режим вече нямат достъп до групово актуализиране и други наследени функции.

> [!IMPORTANT]
> Yammer никога не поддържа импортиране на съдържание в рамките на мрежата, дори когато функцията за експортиране на данни е използвана в друга мрежа. Съдържанието може да бъде повторно Публикувано от партньорски решения или API за почивка на Yammer.

**Експортиране**

[Експортирането на данни на мрежата в мрежата](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) позволява експортирането на съдържание от мрежите на Yammer, включително съобщенията и файловете. Прикачените файлове могат да бъдат изключително големи и ще предизвикат износа, за да се извърши значителен период от време. Препоръчваме активните мрежи да се експортират посредством [API за експортиране на данни](https://developer.yammer.com/docs/data-export-api) на части по ден или седмица. Поддръжката на Microsoft не предоставя скриптове по избор за тази цел.

Съществува отделен [GDPR](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) за експортиране, за да се експортира съдържание за отделен потребител.