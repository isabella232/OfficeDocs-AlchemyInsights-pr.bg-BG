---
title: Проблем при отваряне или изтегляне на файлове в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148185"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Проблем при отваряне или изтегляне на файлове в Yammer

Класически Yammer поддържа няколко варианта за качване на файлове в съобщения и групи. В зависимост от мрежовата конфигурация файловете по подразбиране за съхранение в SharePoint.

Избор на файл в новия Yammer все още не поддържа всички опции, налични в класическия Yammer. Бъдещата актуализация ще добави допълнителни функции. За повече информация вижте [Прикачване на файл или изображение към разговор публикация на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Не може да се отвори или изтегли файл**  

Файлът може да качите в Yammer, но също така да се свързвате към файл в SharePoint Online. За да отстраните проблема, първо трябва да определите местоположението на файла. Ако файлът е качен в Yammer, той ще има *.yammer.com URL. Уверете се, че задължителните URL адреси и IP адреси са отблокирани. За повече информация вижте публикацията [в блога с помощта на твърди кодирани IP адреси за Yammer не се препоръчва](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Проверете дали потребител, който също е глобален администратор може да изтегли файла. Ако файлът е поверително, може да се наложи да използвате режим на лично съдържание. За повече информация вижте [след монитор частно съдържание в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer гости и файлове на ниво мрежа в SharePoint Online**  

[Ниво на мрежата гости в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не използват Azure AD B2B и са вътрешни за услугата Yammer, така че те нямат достъп до Yammer файлове, съхранени в SharePoint. Създаване на външен AAD B2B потребител, който има достъп до библиотеки с документи в SharePoint Online с помощта на тази самоличност. За информация относно бъдещите Azure AD B2B гост поддръжка в Yammer вижте [Business-to-business (B2B) гост поддръжка в Yammer преглед - условия за клиенти и често задавани въпроси](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).