---
title: Как да добавяте и управлявате администратори – Препоръчителни стъпки
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755824"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Как да добавяте и управлявате администратори – Препоръчителни стъпки

Въз основа на вашето описание на проблема намерихме решение за вас. Повечето клиенти могат сами да решат проблема си, след като са следвали нашата документация.

**Редактиране на администратора на абонамента или съ-администратора**

- Администраторът на акаунта може да редактира и двете роли, като има предвид, че администраторът на абонамента може само да променя съвместно администраторите в [портала на Azure](https://ms.portal.azure.com/#home).
- [Добавяне или промяна на администратори на абонаменти за Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Актуализиране на администратора на абонамента или Co-Administrator за вътрешните абонаменти (ИЗЛЪЧВАния)**

Администраторът на услугата или съадминистраторът могат да използват самостоятелно това действие с помощта на следните стъпки:

1. Влезте в портала на [Azure](https://ms.portal.azure.com/#home) и щракнете върху **управление на разходите + плащане** в левия нож.
2. Щракнете върху договорения ред с абонамента си. Това отваря общия преглед на вашия абонамент.
3. В Блейд за **абонамента** щракнете върху **свойства**. 
4. Щракнете върху бутона **администратор на услуга** .
5. Въведете имейла на потребителя, когото искате да зададете като администратор на услугата, и щракнете върху **OK**.

**Добавяне/промяна/премахване на съвместно управление**

1. Влезте в портала на [Azure](https://ms.portal.azure.com/#home) като администратор на услуга.
2. Отваряне [на абонаменти](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) и избиране на план. (CO-adminstrators може да бъде присвояван само в обхвата на абонамента.)
3. Навигиране до " **управление на достъпа" (IAM)**  >  **Classic администраторите**  >  **добавят**  >  **Добави съадминистратор** , за да отворите екрана **Добавяне на съвместно администриране** (ако опцията Добавяне на съвместно администриране е забранена, това означава, че нямате разрешения).
4. Изберете потребителя, когото искате да добавите, и щракнете върху **Добави**.

**Научете повече:**
- [Добавяне на съ-администратор](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Премахване на съ-администратор](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Промяна на администратора на услугата](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Преглед на администратора на акаунт](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Управление на достъпа чрез RBAC и Azure Portal](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Добавяне/изтриване на потребители, използващи Azure Active Directory (AD)**

Можете да добавяте нови потребители или да изтривате съществуващи потребители от вашата организация на Azure Active Directory (Azure AD):

1. За да добавите нов потребител, влезте в портала на [Azure](https://ms.portal.azure.com/#home) като администратор на потребителя за организацията.
2. Изберете **Azure Active Directory**, изберете **потребители** и след това щракнете върху **нов потребител**.
3. На страницата **User** попълнете необходимата информация. Щракнете върху **Създай**. Потребителят се създава и добавя към вашия клиент на Azure AD.

**Научете повече**:

- [Добавяне на нов потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Изтриване на потребител](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Добавяне или актуализиране на информация за потребителския профил чрез Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Препоръчвани документи**

- [Какво представлява базираното на роли управление на достъпа (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Разбиране на различните роли в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Разрешения за роля на администратор в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Урок: предоставяне на достъп за потребител чрез RBAC и портал на Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Отстраняване на проблеми с RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Организиране на вашите ресурси с групи за управление на Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Как да поискате копие на Azure фактура по имейл](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Как да добавите, актуализирате или премахнете кредитна или дебитна карта от Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Управление (повторно активиране/отмяна/превключване) на абонамент](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



