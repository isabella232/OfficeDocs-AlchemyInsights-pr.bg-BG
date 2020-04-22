---
title: 2491 предупреждава имейл съобщения от "Phish доставени поради клиент или потребител замени"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758897"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="7d783-102">Предупреждаване на имейл съобщения от "Phish доставени поради клиент или потребител замени"</span><span class="sxs-lookup"><span data-stu-id="7d783-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="7d783-103">Правилата за предупреждение по подразбиране, наречена "Phish доставени поради клиент или потребител замени" е бил реализиран на клиент с Лицензи за Office 365 ATP P1 и P2.</span><span class="sxs-lookup"><span data-stu-id="7d783-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="7d783-104">Ако сте получили това предупреждение, ето стъпките за разследване:</span><span class="sxs-lookup"><span data-stu-id="7d783-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="7d783-105">От предупредителното съобщение щракнете върху **Преглед на предупреждението,** за да отидете на страницата **"Предупреждения"** в Центъра за сигурност & съответствие.</span><span class="sxs-lookup"><span data-stu-id="7d783-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="7d783-106">Изберете предупреждението, за да видите опцията за Преглед на **списъка със съобщения** или Преглед на **съобщенията в Explorer**.</span><span class="sxs-lookup"><span data-stu-id="7d783-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="7d783-107">И двете опции ви отведат до подробности за съобщението, което включва ИД на съобщението.</span><span class="sxs-lookup"><span data-stu-id="7d783-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="7d783-108">Обърнете внимание, че връзката Threat Explorer автоматично ще филтрира съобщенията, които отговарят на критериите за предупреждение.</span><span class="sxs-lookup"><span data-stu-id="7d783-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="7d783-109">Може да се наложи да настроите филтъра за дата в Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="7d783-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="7d783-110">Фишинг съобщението е доставено поради ръчно конфигурирана отмяна:</span><span class="sxs-lookup"><span data-stu-id="7d783-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="7d783-111">Разрешен подател или домейн, зададен от потребителя.</span><span class="sxs-lookup"><span data-stu-id="7d783-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="7d783-112">Разрешен подател или домейн, зададен от администратора в правилата за антиспам.</span><span class="sxs-lookup"><span data-stu-id="7d783-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="7d783-113">Разрешен IP адрес във връзка с правилата за филтриране.</span><span class="sxs-lookup"><span data-stu-id="7d783-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="7d783-114">Правило за пощенски поток (известен още като транспортно правило), който е конфигуриран да разрешава съобщения в.</span><span class="sxs-lookup"><span data-stu-id="7d783-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="7d783-115">Ако смятате, че съобщението е неправилно маркирани като фиш, използвайте [добавката Outlook съобщение за съобщаване](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) да изпратите съобщение образци на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7d783-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
