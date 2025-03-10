---
title: Намиране на липсващи приложения в острието за регистриране на приложения
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057091"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Намиране на липсващи приложения в острието за регистриране на приложения

1. Не могат да се намерят приложения в портала за регистрация на приложения.

    Ако дадено приложение е много клиентско приложение и е регистрирано в друг клиент, то няма да се показва под "Регистрационен диск за приложения". Можете обаче да го намерите под Enterprise Applications blade, след като е бил достъпен (след като е бил съгласен) и директорът на услугата е създаден във вашия клиент. За повече информация вижте Приложения [& на услуги в Azure AD – Платформа за самоличност на Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Не можете да преглеждате приложения в "Регистрационен диск за приложения", въпреки че сте администратор.

    Уверете се, че сте в правилния указател в портала на Azure.
3. Моето приложение не е в списъка под Enterprise Applications blade, но се показва, когато заядвам командата PowerShell.

    Понякога, след като изтриете приложението от портала на Azure, то не се показва в портала, но може да не е изтрито напълно. За повече информация вижте:
    - Можете да извлечете списъка с по-рано изтрити приложения и да видите дали приложението се показва в списъка с помощта на командата Powershell: **Get-AzureADDeletedApplication**. За да научите повече, [вижте Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Ако искате да премахнете приложението напълно, можете да опитате следното в PowerShell: **Remove-AzureADApplication -ObjectId**. За да научите повече, [вижте Премахване на AzureADПриложение (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Като алтернатива, можете да опитате да възстановите изтритото приложение, като използвате следната команда powershell: **Възстановяване на AzureADDeletedApplication -ObjectId**. За да научите повече, вижте [Възстановяване-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Не мога да намеря списък на всички предварително инсталирани корпоративни приложения в моя нов клиент на Azure.

    По подразбиране няма предварително инсталирани корпоративни приложения в Azure AD. Трябва да го добавите ръчно от опцията "Ново приложение", като го прегледате от галерията на Azure AD или добавите приложение, което не е галерия. За да научите повече, вижте Бързо започване: Добавяне на приложение [към вашия Azure Active Directory (Azure AD) клиент](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Ако сте глобален администратор, можете лесно да получите достъп до вашите приложения с помощта [на Microsoft 365 app Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Не можете да намерите моите приложения от портала "Моите приложения".

    Уверете се, че приложенията не са скрити на страницата "Моите приложения". За да научите повече, вижте [Колекции (предварителен преглед) в портала "Моите приложения" – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. За да стартирате приложения от портала "Моите [приложения", вижте Намиране & приложения в портала "Моите приложения" – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Приложението Mover не се показва на enterprise Applications blade след инсталирането.

    Приложението "Office 365 Mover" е многотенантно приложение, което не е необходимо да се добавя към AAD, като се използва секцията Приложения на галерията под Enterprise App Registration. За достъп Office 365 Mover, просто влезте в приложението и ще поискате съгласието на потребителя за разрешенията. След като потребителят даде съгласието си, това приложение автоматично ще бъде добавено към клиента с ИД на имейл, който сте влезли.

    След като влезете в приложението, би трябвало да можете да намерите записа на това приложение под острието enterprise Applications в AAD. Трябва да потърсите това приложение, като въведете пълното име, т.е. "Office 365 Mover", или просто да потърсите "office" и то трябва да изброи приложението. За да научите повече, вижте Office 365 Mover казва, че вече е инсталиран, но не е в списъка в [галерията с корпоративни приложения.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. [Quickstart:](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) Преглед на списъка с приложения, които използват вашия клиент на Azure Active Directory (Azure AD) за управление на самоличност, ви показва как да преглеждате приложенията, известни също като приложения, които вече са настроени да използват вашия клиент на Azure AD като свой доставчик на самоличност (IdP).
9. [Отстраняването на често срещан проблем при добавянето](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) или премахването на приложение към Azure Active Directory ви помага да разберете често срещаните проблеми, пред които хората се сблъскват с преглеждането на приложения в Azure Active Directory.
