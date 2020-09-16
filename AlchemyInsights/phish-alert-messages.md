---
title: 2491 известия за имейл съобщения от правилата за "phisher, доставени поради клиент или за заместване на потребители"
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
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728600"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="c3911-102">Информиране на имейл съобщения от правилата на "phisher доставяния поради клиент или за отмяна на потребители"</span><span class="sxs-lookup"><span data-stu-id="c3911-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="c3911-103">За клиенти с Office 365 ATP P1 и P2 се предоставят правила за известия по подразбиране с име "уеб клиент или превключвател за потребители".</span><span class="sxs-lookup"><span data-stu-id="c3911-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="c3911-104">Ако сте получили това известие, ето стъпките, за да изследвате:</span><span class="sxs-lookup"><span data-stu-id="c3911-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="c3911-105">От уведомителното съобщение щракнете върху **Преглед на известяване** , за да отидете на страницата за **предупреждения** в центъра за съответствие на & за защита.</span><span class="sxs-lookup"><span data-stu-id="c3911-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="c3911-106">Изберете известието, за да видите опцията за **Преглед на списъка със съобщения** или да **преглеждате съобщения в Explorer**.</span><span class="sxs-lookup"><span data-stu-id="c3911-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="c3911-107">И двете опции ще ви отведат до подробностите за съобщението, което включва ИД на съобщението.</span><span class="sxs-lookup"><span data-stu-id="c3911-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="c3911-108">Имайте предвид, че връзката за Explorer на заплахите автоматично ще филтрира съобщенията, които отговарят на критериите за уведомяване.</span><span class="sxs-lookup"><span data-stu-id="c3911-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="c3911-109">Може да се наложи да настроите филтъра за дата в Explorer на заплахите.</span><span class="sxs-lookup"><span data-stu-id="c3911-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="c3911-110">Фишинг съобщението е доставено поради ръчно конфигурирани замествания:</span><span class="sxs-lookup"><span data-stu-id="c3911-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="c3911-111">Позволен подател или домейн, зададен от потребителя.</span><span class="sxs-lookup"><span data-stu-id="c3911-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="c3911-112">Позволен подател или домейн, зададено от администратора в правила за нежелана поща.</span><span class="sxs-lookup"><span data-stu-id="c3911-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="c3911-113">Позволен IP адрес в правилата за филтриране на връзката.</span><span class="sxs-lookup"><span data-stu-id="c3911-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="c3911-114">Правило за поток на поща (известно също като транспортно правило), което е конфигурирано да позволява съобщения в.</span><span class="sxs-lookup"><span data-stu-id="c3911-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="c3911-115">Ако смятате, че съобщението е било неправилно маркирано като Фиш, използвайте [добавката за съобщение на отчета](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) за Outlook, за да подадете образци на съобщения на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c3911-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
