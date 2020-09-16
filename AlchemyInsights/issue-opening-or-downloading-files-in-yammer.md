---
title: Проблем при отварянето или изтеглянето на файлове в Yammer
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
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695638"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Проблем при отварянето или изтеглянето на файлове в Yammer

Класическата Yammer поддържа множество опции за качване на файлове в съобщения и групи. В зависимост от конфигурацията на мрежата, файлове по подразбиране за място за съхранение в SharePoint.

Опцията за избор на файл в нови Yammer все още не поддържа всички опции, които са налични в класическата Yammer. Бъдеща актуализация ще добави допълнителни функции. За повече информация вижте [Прикачване на файл или изображение към публикация в разговор на Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Не можете да отворите или изтеглите файл**  

Даден файл може да се качи в Yammer, но също така да се свързва към файл в SharePoint online. За да отстраните проблема, първо трябва да определите местоположението на файла. Ако файлът е качен в Yammer, той ще има URL адрес *. yammer.com. Уверете се, че изискваните URL адреси и IP адреси са Разблокирани. За повече информация вижте публикацията в блог [с помощта на ТРУДНИ IP адреси за Yammer не се препоръчва](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Проверете дали потребител, който е и глобален администратор, може да Изтегли файла. Ако файлът е личен, е възможно да се наложи да използвате частното съдържание. За повече информация вижте [наблюдение на личното съдържание в Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Клиенти и файлове в мрежата на Yammer в SharePoint online**  

[Гостите на ниво мрежа в Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) не използват AZURE ad B2B и са вътрешни за услугата yammer, така че да не могат да имат достъп до файлове на yammer, съхранени в SharePoint. Създаване на външен потребител на потребителски интерфейс, който има достъп до библиотеките с документи в SharePoint Online, с помощта на тази самоличност. За информация относно бъдещия поддръжка на Azure AD B2B за гости в Yammer вижте [поддръжка за гост на фирма за бизнес (B2B) в предварителния преглед на Yammer – общи условия и ЧЗВ за клиенти](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).