---
title: Не може да се Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893900"
---
# <a name="unable-to-activate-office"></a>Не може да се Office

**Забележка:** Ако използвате по-стара версия на Windows (например Windows 7), уверете се, че TLS 1.2 е разрешено по подразбиране. За повече информация вижте Актуализиране, за да [разрешите TLS 1.1 и TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)като защитени протоколи по подразбиране в WinHTTP в Windows.

- Проверете дали срокът на абонамента ви не е изтекъл.
- Уверете се, че имате абонамент, който позволява клиентски лицензи, като Office 365 Business или Бизнес Premium, и се уверете, [че потребителят има присвоен лиценз](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Уверете се, че потребителят влиза в Office със същия акаунт, на който е присвоен лицензът.
- Проверете [Страницата за състояние на услугата Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health), за да видите дали няма някакви известни проблеми с услугата.
- Проверете настройките на защитната стена, антивирусния софтуер и прокси сървъра, за да потвърдите, че те Microsoft 365 блокират достъпа на приложенията до интернет. Вижте [Диапазони на URL и IP адреси за Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Диапазони от URL и IP адреси за Office 365").

**Съвет** На Windows можем да диагностицираме и автоматично да коригираме няколко често срещани Office за влизане. Изтеглете и стартирайте **[microsoft Помощник за поддръжка и възстановяване,](https://aka.ms/SaRA-OfficeSignInScenario)** за да използвате нашия автоматизиран инструмент.

Използвайте следните действия за отстраняване на проблеми:

- Отворете приложение на Office и [излезте](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) от всички съществуващи потребителски акаунти. [Премахнете](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) и [дайте повторно](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) лиценз за Office, а след това [влезте в Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) като използвате засегнатия потребителски акаунт.
- Изпълнение на [Програмата за отстраняване на проблеми при активиране](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Нулиране на състоянието на активиране на Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Нулиране на Office на активиране")
- [Извършване на онлайн поправка на Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

За допълнителни решения за отстраняване на проблеми вижте:  

- [Грешки поради нелицензиран продукт и грешки при активиране на Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [Грешка при активиране на Office. "За съжаление, не можем да се свържем с вашия акаунт. Опитайте отново по-късно"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)