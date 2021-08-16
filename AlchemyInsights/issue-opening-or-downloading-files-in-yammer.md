---
title: Проблем при отваряне или изтегляне на файлове в Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028239"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Проблем при отваряне или изтегляне на файлове в Yammer

Класическата Yammer поддържа множество опции за качване на файлове в съобщения и групи. В зависимост от конфигурацията на мрежата файловете по подразбиране за съхранение в SharePoint.

Програмата за избор на файлове в Yammer все още не поддържа всички опции, налични в класическия Yammer. Бъдещата актуализация ще добави допълнителни функции. За повече информация вижте [Прикачване на файл или изображение към публикация Yammer разговор.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**Не може да се отвори или изтегли файл**  

Файлът може да се качи Yammer, но също така да се свързва към файл в SharePoint Online. За отстраняване на неизправности първо трябва да определите местоположението на файла. Ако файлът е качен в Yammer, той ще има *.yammer.com URL адрес. Уверете се, че задължителните URL адреси и IP адреси са разблокирани. За повече информация вижте публикацията в [блога Използване на твърди кодирани IP адреси за Yammer не се препоръчва.](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)

Проверете дали потребител, който е и глобален администратор, може да изтегли файла. Ако файлът е личен, може да се наложи да използвате режима на частно съдържание. За повече информация вижте След това [Наблюдавайте личното съдържание в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer на ниво мрежа и файлове в SharePoint Онлайн**  

[Гостите на мрежово ниво в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не използват Azure AD B2B и са вътрешни за услугата Yammer, така че нямат достъп до Yammer файлове, съхранени в SharePoint. Създайте външен потребител на AAD B2B, който има достъп до библиотеки с документи в SharePoint Онлайн с помощта на тази самоличност. За информация за бъдеща поддръжка за гости на Azure AD B2B в Yammer вж. Поддръжка за гости от бизнес към бизнес [(B2B) в Yammer предварителен преглед – Условия на клиентите и ЧЗВ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).