---
title: Липсващи имейли под карантина
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
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892036"
---
# <a name="missing-emails-in-quarantine"></a>Липсващи имейли под карантина

Администраторите могат [да преглеждат, пускат или изтриват тези съобщения](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

В портала Microsoft 365 Defender отидете на <https://security.microsoft.com> Преглед на **карантината.** \>  Или, за да отидете директно на страницата **Карантина,** използвайте <https://security.microsoft.com/quarantine> .  

За повече информация относно стойностите за търсене/филтриране, които можете да използвате, вижте Управление на съобщения и файлове под карантина [като администратор в EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files).

Кратките команди, които използвате за преглед и управление на съобщения и файлове под карантина, са:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Експортиране-карантинаMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Обърнете внимание, че тази кратка команда е само за съобщения, а не за файлове от Сейф Прикачени файлове за SharePoint, OneDrive или Microsoft Teams.
- [Съобщение за карантинаMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
