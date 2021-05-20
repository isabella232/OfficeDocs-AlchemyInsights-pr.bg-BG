---
title: 2491 Известяване на имейл съобщения от правилата "Фишинг доставяни поради клиент или заместване на потребител"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544567"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="78a94-102">Известяване на имейл съобщения от правилата за "Фишинг, доставен поради заместване на клиент или потребител"</span><span class="sxs-lookup"><span data-stu-id="78a94-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="78a94-103">Правилата за известяване по подразбиране, наречени "Фишинг доставяни поради клиент или потребителски приоритет", са били предоставени на клиента с лицензи на Microsoft Defender за Office 365 P1 и P2 лицензи.</span><span class="sxs-lookup"><span data-stu-id="78a94-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="78a94-104">Ако сте получили това известие, ето стъпките, които трябва да проучите:</span><span class="sxs-lookup"><span data-stu-id="78a94-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="78a94-105">От предупредителното съобщение щракнете върху **Преглед на предупреждението,** за да отидете **на** страницата Известия в центъра за & съответствие.</span><span class="sxs-lookup"><span data-stu-id="78a94-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="78a94-106">Изберете известието, за да видите опцията за Преглед **на списъка със съобщения** или Преглед на съобщения в **Explorer**.</span><span class="sxs-lookup"><span data-stu-id="78a94-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="78a94-107">И двете опции ще ви откарат до подробностите за съобщението, което включва ИД на съобщението.</span><span class="sxs-lookup"><span data-stu-id="78a94-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="78a94-108">Обърнете внимание, че връзката Threat Explorer автоматично ще филтрира съобщенията, които отговарят на критериите за известяване.</span><span class="sxs-lookup"><span data-stu-id="78a94-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="78a94-109">Може да се наложи да настроите филтъра за дата в Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="78a94-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="78a94-110">Фишинг съобщението е доставено поради ръчно конфигурирано заместване:</span><span class="sxs-lookup"><span data-stu-id="78a94-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="78a94-111">Разрешен подател или домейн, зададен от потребителя.</span><span class="sxs-lookup"><span data-stu-id="78a94-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="78a94-112">Разрешен подател или домейн, зададен от администратора в правила за нежелана спам.</span><span class="sxs-lookup"><span data-stu-id="78a94-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="78a94-113">Разрешен IP адрес в правилата за филтриране на връзка.</span><span class="sxs-lookup"><span data-stu-id="78a94-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="78a94-114">Правило за пощенския поток (известно още като транспортно правило), което е конфигурирано да разрешава съобщения.</span><span class="sxs-lookup"><span data-stu-id="78a94-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="78a94-115">Ако смятате, че съобщението е маркирано неправилно като фиш, използвайте добавката Outlook [съобщение](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) за отчет, за да подадете образци на съобщения до Microsoft.</span><span class="sxs-lookup"><span data-stu-id="78a94-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
