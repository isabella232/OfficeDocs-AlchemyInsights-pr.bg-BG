---
title: Моето приложение не се показва в управлението на приложения
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454428"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Моето приложение не се показва в управлението на приложения

Ако вашето приложение не се показва в управлението на приложения, проверете следното:

1. Отидете в [Azure AD](https://aad.portal.azure.com/) и намерете ИД на приложението за вашето приложение, като потърсите името на приложението в горната лента на страницата Общ преглед.

1. Access Graph Explorer и потърсете ИД на приложение в рамките на вашата основна услуга, като използвате тази заявка и заместите със съответния ИД на <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? приложение: $search= "AppId: <appId> ">

1. Ако не се върнат резултати, потърсете ИД на приложение в приложението, като използвате тази заявка и заместите със съответния ИД на <appId> приложение: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Ако имате проблеми със заявката, вижте Получаване [на поддръжка](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

За повече информация или прозрения за вашите приложения в управлението на приложения вижте [Научете повече за видимостта и прозренията.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

За повече информация относно преглеждането на приложенията вижте [Преглед на приложенията.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
