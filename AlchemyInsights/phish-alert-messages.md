---
title: 2491 сигнала имейл съобщения от политиката на "Phish доставено поради наемател или ползвател отмяна"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391116"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="0670c-102">Сигнала имейл съобщения от политиката на "Phish доставено поради наемател или ползвател отмяна"</span><span class="sxs-lookup"><span data-stu-id="0670c-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="0670c-103">По подразбиране предупреждение правилото с име "Phish предоставените поради наемател или ползвател пренебрегване" е разточва на наематели с Office 365 ATP P1 и P2 лицензи.</span><span class="sxs-lookup"><span data-stu-id="0670c-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="0670c-104">Ако сте получили този сигнал, тук са стъпките, за да разследва:</span><span class="sxs-lookup"><span data-stu-id="0670c-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="0670c-105">От определителен член предупреждение съобщение щракнете върху **Изглед сигнал** да отидете на страницата на **сигналите** в защита & съответствие център.</span><span class="sxs-lookup"><span data-stu-id="0670c-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="0670c-106">Изберете предупреждението да видите опция за **изглед на списъка със съобщения** или **съобщения за преглед в Explorer**.</span><span class="sxs-lookup"><span data-stu-id="0670c-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="0670c-107">И двете от тези опции да ви отведе до подробностите на съобщението, което включва ИД на съобщение.</span><span class="sxs-lookup"><span data-stu-id="0670c-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="0670c-108">Обърнете внимание, че заплахата изследовател връзката автоматично ще филтрира съобщенията, които отговарят на критериите за предупреждение.</span><span class="sxs-lookup"><span data-stu-id="0670c-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="0670c-109">Трябва да настроите филтъра "дата" в заплахата изследовател.</span><span class="sxs-lookup"><span data-stu-id="0670c-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="0670c-110">Фишинг съобщението е доставено поради ръчно конфигуриран замени:</span><span class="sxs-lookup"><span data-stu-id="0670c-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="0670c-111">Разрешени подател или домейн, зададен от потребителя.</span><span class="sxs-lookup"><span data-stu-id="0670c-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="0670c-112">Разрешени подател или домейн, зададен от администратор в анти-спам политика.</span><span class="sxs-lookup"><span data-stu-id="0670c-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="0670c-113">Разрешените IP адрес с връзка филтър политика.</span><span class="sxs-lookup"><span data-stu-id="0670c-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="0670c-114">Пощенски поток правило (известен също като транспортно правило) е конфигуриран да разрешава съобщения в.</span><span class="sxs-lookup"><span data-stu-id="0670c-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="0670c-115">Ако смятате, че съобщението е неправилно маркирани като phish, използвайте Outlook [добавката към съобщението](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) да представи съобщение проби на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0670c-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
