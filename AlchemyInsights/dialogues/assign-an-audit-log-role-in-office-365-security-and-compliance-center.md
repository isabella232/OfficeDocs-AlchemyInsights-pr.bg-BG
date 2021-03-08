---
title: Присвояване на роля на регистрационен файл за проверка в центъра за съответствие на & за защита на Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 03/05/2021
ms.locfileid: "50523523"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="62fac-102">Присвояване на роля на регистрационен файл за проверка в центъра за съответствие на & за защита на Office 365</span><span class="sxs-lookup"><span data-stu-id="62fac-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="62fac-103">За да търсите в регистрационния файл за проверка на Office 365, на администратора трябва да е присвоена ролята на **регистрационни файлове за проверка само за преглед** или ролята на **регистрационни файлове за проверка** в Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="62fac-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="62fac-104">Тези роли се задават на ролевите групи за управление на съответствието и на организацията по подразбиране.</span><span class="sxs-lookup"><span data-stu-id="62fac-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="62fac-105">Глобалните администратори в Office 365 и Microsoft 365 се добавят автоматично като членове на ролевата група за управление на организацията.</span><span class="sxs-lookup"><span data-stu-id="62fac-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="62fac-106">За да разрешите на потребителя да търси с минималното ниво на привилегии, Създайте потребителска ролева група в Exchange Online, добавете ролята за **регистрационни файлове за проверка само за преглед** или ролята на **регистрационни файлове за проверка** и след това добавете потребителя като член на новата ролева група.</span><span class="sxs-lookup"><span data-stu-id="62fac-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="62fac-107">За повече информация вижте [управление на ролеви групи в Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) и [търсене в регистрационния файл за проверка в центъра за съответствие на защитата &](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span><span class="sxs-lookup"><span data-stu-id="62fac-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>