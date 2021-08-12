---
title: Как да добавяте и управлявате администратори – препоръчителни стъпки
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 5aa6f11d31ed62078fdd05090af5722289544c5ab2244a369182f4e0f9214183
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963776"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Как да добавяте и управлявате администратори – препоръчителни стъпки

Въз основа на описанието на проблема ви открихме решение за вас. Повечето клиенти са били в състояние да разрешат проблема си сами, след като са следвали нашата документация.

**Редактиране на администратора на абонамента или съ администратора**

- Администраторът на акаунта може да редактира и двете роли, докато администраторът на абонамента може да променя само съ администраторите в [портала на Azure.](https://ms.portal.azure.com/#home)
- [Добавяне или промяна на администратори на абонаменти за Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Актуализиране на абонаментния администратор или Co-Administrator за вътрешни (AIRS) абонаменти**

Администраторът на услугата или съ администраторът могат самостоятелно да служат на това действие с помощта на следните стъпки:

1. Влезте в портала [на Azure и щракнете](https://ms.portal.azure.com/#home) върху Управление на разходите + **Фактуриране** в левия диск.
2. Щракнете върху елемента на реда с вашия абонамент. Това отваря общ преглед за вашия абонамент.
3. В **острието Абонамент** щракнете върху **Свойства**. 
4. Щракнете върху бутона **Администратор на** услугата.
5. Въведете имейла на потребителя, когото искате да зададете като администратор на услугата, и щракнете върху **OK**.

**Добавяне/промяна/премахване на съ-администратор**

1. Влезте в портала [на Azure](https://ms.portal.azure.com/#home) като администратор на услугата.
2. Отворете [Абонаменти](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и изберете абонамент. (Съ-администраторите могат да бъдат присвоявани само в обхвата на абонамента.)
3. Отидете до Управление на **Access (IAM)** Класически администратори Добавяне на съ-администратор, за да отворите екрана Добавяне на съ-администратор (Ако опцията Добавяне на  >    >    >   съ-администратор е забранена, тя означава, че не разполагате с разрешения). 
4. Изберете потребителя, когото искате да добавите, и щракнете върху **Добави**.

**Научете повече:**
- [Добавяне на съ-администратор](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Премахване на съ администратор](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Промяна на администратора на услугата](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Преглед на администратора на акаунта](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Управление на достъпа с помощта на портала на RBAC и Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Добавяне/изтриване на потребители чрез Azure Active Directory (AD)**

Можете да добавяте нови потребители или да изтривате съществуващи потребители от вашата Azure Active Directory (Azure AD):

1. За да добавите нов потребител, влезте в [портала на Azure](https://ms.portal.azure.com/#home) като администратор на потребителя за организацията.
2. Изберете **Azure Active Directory**, изберете **Потребители и** след това щракнете върху Нов **потребител**.
3. На страницата **Потребител** попълнете необходимата информация. Щракнете **върху Създаване**. Потребителят се създава и добавя към вашия клиент на Azure AD.

**Научете повече:**

- [Добавяне на нов потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Изтриване на потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Добавяне или актуализиране на информация за потребителски профил чрез Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Препоръчителни документи**

- [Какво представлява контролата за достъп, базирана на роли (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Разбиране на различните роли в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Разрешения за администраторска роля в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Урок: Предоставяне на достъп за потребител с помощта на RBAC и портала на Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Отстраняване на неизправности с RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Организиране на ресурсите с групи за управление на Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Как да поискате копие на фактура на Azure по имейл](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Как да добавите, актуализирате или премахнете кредитна или дебитна карта от Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Абонамент за управление (повторно активиране/отказ/превключване)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



