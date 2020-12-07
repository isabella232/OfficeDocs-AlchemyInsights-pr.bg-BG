---
title: Поддръжката на Microsoft Edge за Microsoft Defender Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583250"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Поддръжката на Microsoft Edge за Microsoft Defender Guard

Предназначена за Windows 10 и Microsoft Edge, Guard използва хардуерна изолация подход, който позволява на потребителя да навигира в ненадежден сайт от изолиран, Хипер-V контейнер, отделен от операционната система.

Корпоративен администратор определя списък с надеждни уеб сайтове, ресурси в облака и вътрешни мрежи. Когато потребител посети сайт, който не е в списъка, Microsoft Edge ще отвори сайта в контейнера. Това означава, че ако сайтът се окаже злонамерен, хост КОМПЮТЪРЪТ ще остане защитен и атакуващият няма да стигне до корпоративните данни.

Инсталирането на разширения в контейнера се поддържа като версия на Microsoft Edge 81 и може да се управлява чрез правилата. Адресът на updateURL, който се използва в политиката на ExtensionInstallForcelist, трябва да бъде добавен като неутрален ресурс в правилата за изолация на мрежата, използвани от Guard за приложения.

За повече информация вижте [поддръжка на Microsoft Edge за Microsoft Defender Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
